# Kuzushiji-MNIST
Repository for Kuzushiji_MNIST, Kuzushiji49, and Kuzushiji_Kanji

![Image showing examples of each class of Kuzushiji MNIST](https://storage.googleapis.com/kuzushiji-mnist/kuzushiji_mnist.png)

## Get the data
### Kuzushiji-MNIST

Kuzushiji-MNIST contains 70,000 28x28 grayscale images spanning 10 classes (one from each column of [hiragana](https://upload.wikimedia.org/wikipedia/commons/thumb/2/28/Table_hiragana.svg/768px-Table_hiragana.svg.png) except ん), and is perfectly balanced like the original MNIST dataset (6k/1k train/test for each class).

| File            | Number of examples | Download (MNIST format)    | Download (NumPy format)      |
|-----------------|--------------------|----------------------------|------------------------------|
| Training images | 60,000             | train-images-idx3-ubyte.gz | kuzushiji10-train-imgs.npy   |
| Training labels | 60,000             | train-labels-idx1-ubyte.gz | kuzushiji10-train-labels.npy |
| Testing images  | 10,000             | t10k-images-idx3-ubyte.gz  | kuzushiji10-test-imgs.npy    |
| Testing labels  | 10,000             | t10k-labels-idx1-ubyte.gz  | kuzushiji10-test-labels.npy  |

##### Which format do I download?
If you're looking for a drop-in replacement for the MNIST or Fashion-MNIST dataset (for tools that currently work with these datasets), download the data in MNIST format.

Otherwise, it's recommended to download in NumPy format, which can be loaded into an array as easy as:  
`arr = np.load(filename)`.
