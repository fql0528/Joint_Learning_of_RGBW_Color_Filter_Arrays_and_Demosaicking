# Joint Learning of RGBW Color Filter Arrays and Demosaicking
#### Chenyan Bai, Faqi Liu, Jia Li
>RGBW color filter arrays (CFAs) have gained widespread attention for their superior performance in low-light conditions. Most existing demosaicking methods are tailored for specific RGBW CFAs or involve manual joint design with CFAs. The close relationship between sampling and reconstruction means that restricting the search space through predefined CFAs and demosaicking methods severely limits the ability to achieve optimal performance. In this paper, we propose a new approach for joint learning of RGBW CFA and demosaicking. This approach can simultaneously learn optimal CFAs and demosaicking methods of any size, while also being capable of reconstructing mosaicked images of any size. We use a surrogate function and arbitrary CFA interpolation to ensure end-to-end learning of the RGBW CFA. We also propose a dual-branch fusion reconstruction network that utilizes the W channel to guide the reconstruction of R, G, and B channels, reducing color errors while preserving more image details. Extensive experiments demonstrate the superiority of our proposed method.

## Environment installation
We use PyTorch for training, and use custom convolutional layers to simulate RGBW CFA design and demosaicing.Assuming you have [Anaconda](https://www.anaconda.com/products/individual#Downloads):
```bash
conda create -n learncfa python=3.7
conda activate learncfa
```
