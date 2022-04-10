<center>

# Biological Learning

A GPU implementation of [Biological Learning](https://github.com/DimaKrotov/Biological_Learning). This is a fork from [this repo](https://github.com/DimaKrotov/Biological_Learning) by D. Krotov and J. Hopfield.

|<img src="https://user-images.githubusercontent.com/79289947/156650751-33da2304-cf57-4880-b51b-dc21e6a5f549.gif" width="200" height="200"/> | <img src="https://user-images.githubusercontent.com/79289947/156464655-c226dc9f-a93a-4c17-ab91-b20145b32d7f.gif" width="200" height="200"/> | <img src="https://user-images.githubusercontent.com/79289947/156464703-3d20ebc0-3a21-4532-b2f6-03279a524021.gif" width=200 height=200/> |
|:---:|:---:|:---:
| MNIST |CIFAR-10 | Real/Fake Faces |
</center>

## Structure


### Notebooks:
- [**Unsupervised_learning_algorithm_MNIST.ipynb**](Unsupervised_learning_algorithm_MNIST.ipynb): Compares the BIO algorithm with backprop (BP) model on the MNIST dataset for digit recognition. 

- [**CIFAR-10, + gpu implementation for bio-unsupervised.ipynb**](https://github.com/heydarshahi/Biological_Learning/blob/master/CIFAR-10%2C%20%2B%20gpu%20implementation%20for%20bio-unsupervised.ipynb ): A comparison between BIO and BP models for object classification on CIFAR-10 dataset.

- [**Face detection.ipynb**](https://github.com/heydarshahi/Biological_Learning/blob/master/Face%20detection.ipynb): Real/Fake Face classification.
- [**Unsupervised learning on Face (Gender, Ethicity)**](https://github.com/heydarshahi/Biological_Learning/blob/master/Unsupervised%20learning%20on%20Face%20(Gender%2C%20Ethicity).ipynb): Gender and ethnicity classification.


## Installation
We create a conda environment using  `environment.yml`. Feel free to change the package versions. To install the environment:

```bash
conda env create -f environment.yml
conda env list 
conda activate hebbian 
```
**Note:** To get the best of GPU functionalities, you should have a cuda-compatible gpu. Please change the `cudatoolkit`, `tensorflow`, and `pytorch` versions to match your GPU settings.


## Running the Code
To run any of the notebooks, simply run:
```bash
jupyter notebook [NOTEBOOK NAME]
```

## Results
### MNIST:
<center>

| N_hid | BIO Validation Accuracy | BP Validation Accuracy |
|:-----:|:-----------------------:|:----------------------:|
|  200  |           95.7          |          97.9          |
|  500  |           96.5          |          97.9          |
|  1000 |           97.2          |          98.1          |
|  2000 |           97.8          |          98.15         |
|  4000 |           98.1          |          98.29         |
|  8000 |           98.1          |          98.3          |

|<img src="https://user-images.githubusercontent.com/79289947/156661813-fd3a04f2-65c1-41a3-a46b-c05c088704d7.png" width="500" height="300"/>  | <img src="https://user-images.githubusercontent.com/79289947/156650751-33da2304-cf57-4880-b51b-dc21e6a5f549.gif" width="240" height="240"/> |
|:----:|:----:|
|BIO vs. BP Accuracies for MNIST | BIO Weights Visualization |

</center>


### CIFAR-10:
<center>

| N_hid | BIO Validation Accuracy | BP Validation Accuracy |
|:-----:|:-----------------------:|:----------------------:|
|  1000 |           46.5          |          54.2          |
|  2000 |           49.0          |          54.2          |
|  4000 |           50.3          |          54.6         |
|  8000 |           52.0          |          55.0          |

| <img src="https://user-images.githubusercontent.com/79289947/156664660-d3065024-45b8-41c3-b5a9-5afac6885e5b.png" width="500" height="300"/>  | <img src="https://user-images.githubusercontent.com/79289947/156464655-c226dc9f-a93a-4c17-ab91-b20145b32d7f.gif" width="240" height="245"/> |
|:----:|:----:|
|BIO vs. BP Accuracies for CIFAR | BIO Weights Visualization |

</center>


## Resources
Example of "biological" learning for MNIST based on the paper [Unsupervised Learning by Competing Hidden Units](https://doi.org/10.1073/pnas.1820458116) by D.Krotov and J.Hopfield. If you want to learn more about this work you can also check out this [lecture](https://www.youtube.com/watch?v=4lY-oAY0aQU) from MIT's [6.S191 course](http://introtodeeplearning.com/).  

## Author and License
(c) 2018 Dmitry Krotov
-- Apache 2.0 License

This fork is the work of Yana Kuznetcov and Amin Heydarshahi and was initially developed as the course project for the graduate class Computational Visual Perception, instructed and supervised by [Prof. Dr. Bernhard Egger](https://eggerbernhard.ch/) and  [Dr. Patrick Krauß](https://www.ai.fau.digital/speakers/dr-patrick-kraus/). 
