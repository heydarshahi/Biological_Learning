# Biological_Learning
Example of "biological" learning for MNIST based on the paper [Unsupervised Learning by Competing Hidden Units](https://doi.org/10.1073/pnas.1820458116) by D.Krotov and J.Hopfield. If you want to learn more about this work you can also check out this [lecture](https://www.youtube.com/watch?v=4lY-oAY0aQU) from MIT's [6.S191 course](http://introtodeeplearning.com/).  

|<img src="https://user-images.githubusercontent.com/79289947/156466084-2c5f3cca-b8ac-4e77-9597-09e5982f8ead.gif" width="170" height="170"/> | <img src="https://user-images.githubusercontent.com/79289947/156464655-c226dc9f-a93a-4c17-ab91-b20145b32d7f.gif" width="170" height="170"/> | <img src="https://user-images.githubusercontent.com/79289947/156464676-d5b88f0f-0338-47f0-b7cb-fb55489a48ae.gif" width=170 height=170/> |<img src="https://user-images.githubusercontent.com/79289947/156464703-3d20ebc0-3a21-4532-b2f6-03279a524021.gif" width=170 height=170/> |
|---|---|---|---|



## Getting started

Install jupyter notebook and numpy, scipy, matplotlib.

```bash
> jupyter notebook
```
Run any of the 4 notebooks, observe weights, train BIO and BP models, create your own experiments:
- Unsupervised MNIST models
- CIFAR10 BIO models
- Unsupervised learning on Faces
- Face detection with CNNs

## Dependencies

- Use `environment.yml` to create an Anaconda environment:
- `conda env create -f environment.yml`
- **Note:** To get the best of GPU functionalities, you should have a cuda-compatible gpu. Please change the `cudatoolkit`, `tensorflow`, and `pytorch` versions to match your GPU settings.

## Author and License
(c) 2018 Dmitry Krotov
-- Apache 2.0 License
