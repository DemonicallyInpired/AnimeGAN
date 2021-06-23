## AnimeGAN &mdash; A Use-Case Implementation for StyleGAN2
*This project deals with generating Anime Character in particular the female Anime Character with a StyleGAN variant of all the fascinating version of Generative Adverserial Network introduced in the past. Though a head tonne of fascinating variant of GAN has came along in the past decade like cycle GAN or DCGAN, almost none has produced promising results that can stand in par with industry standards when it comes to generating eastern animation style character often know as Anime. However, the recent spur of a rather new addition to this already proliferating domain of GANs i.e. the Style GAN introduced by Nvidia Labs has almost make it possible to push aside the boundaries of trade-off between the quality and the relevance of the generated objects.*

## Requirements:
* Linux or Windows(10 or newer) operating System
* 64-bits Python 3.6 installation
* Numpy v1.14.3 or newer
* Tensorflow v1.14 or v1.15
* CUDA 10.0 toolkit and cuDNN 7.5
* CUDA NVCC for seperate compilation

```
The proposed model for this project is trained on a VM instance on AWS with px2.large instance with the above-mentioned specifications
```
## Generated sample image in the latent Space
![Teaser image](./out/output.png)


## Project Structure

```
AnimeGAN/
├── AnimeGAN.ipynb
(Main Driver Code)          
├── out                     
│   ├── mov.mp4
    (Interpolation in the latent space)
│   └── output.png
        (Projection of images in the latent Space)
├── README.md
└── stylegan2
(official Stylegan2 Utilities)
```
## Dataset
Most of our dataset has been scrapped from [getchu](http://www.getchu.com/), a website that provides information about anime and Japanese games, and each of them have a character introduction page, which has a still image of a character along with the description of the character.

## Interpolation Loop
![](out/mov.gif)

## Acknowledgements

This work is largely dependent on Nvidia Labs's implementation of StyleGAN2, and we acknowlege all the contributors for the core implementation of the StyleGAN2 architecture, our work just explore one of the possible implementation of StyleGAN in generating Anime Characters.
