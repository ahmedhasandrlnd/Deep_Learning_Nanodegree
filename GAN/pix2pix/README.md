# Lesson 3: Pix2Pix and CycleGAN

## Concepts

1. [Introducing Jun-Yan Zhu](https://www.youtube.com/watch?time_continue=3&v=l8sCN1rMt6E)
1. [Image to Image Translation](https://www.youtube.com/watch?time_continue=2&v=f-WnvKQd10k)
	1. Ian Goodfellow's [original paper on GANs](http://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf)
	1. Face swap with [CycleGAN Face-off](https://arxiv.org/pdf/1712.03451.pdf)
1. [Designing Loss Functions](https://www.youtube.com/watch?time_continue=4&v=YL1kKWHr7Gc)
	> The objective function we've used the most in this program is cross entropy loss, which is a negative log loss applied to the output of a softmax layer. For a binary classification problem, as in real or fake image data, we can calculate the binary cross entropy loss as:
	> -[y\log(\hat{y})+(1-y)\log(1-\hat{y})	
	In other words, a sum of two log losses!
1. [GANs, a Recap](https://www.youtube.com/watch?time_continue=2&v=MEKTiR1Xkjg)
	> a latent vector is just a compressed, feature-level representation of an image!
	> This manipulation of latent space has even been used to create an [interactive GAN, iGAN](https://github.com/junyanz/iGAN/blob/master/README.md) for interactive image generation! I recommend reading the paper, linked in the Github readme.
1. [Pix2Pix Generator](https://www.youtube.com/watch?time_continue=1&v=94Kml3ekrUI)
	> If you're interested in learning more, take a look at the [original Pix2Pix paper](https://arxiv.org/pdf/1611.07004.pdf). I'd also recommend this related work on creating high-res images: [high resolution, conditional GANs](https://tcwang0509.github.io/pix2pixHD/).
1. [Pix2Pix Discriminator](https://www.youtube.com/watch?v=3Khqf7WtCxY)
	> Try out Christopher Hesse's [image-to-image demo](https://affinelayer.com/pixsrv/) to get some really interesting (and sometimes creepy) results!
1. [CycleGANs & Unpaired Data](https://www.youtube.com/watch?time_continue=17&v=-fbaRaXDqMY)
	> Many of these image are collected in the [Pix2Pix and CycleGAN Github repo](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix) developed by Jun-Yan.
	And you can read the [CycleGAN paper, here](https://arxiv.org/pdf/1703.10593.pdf).
1. [Cycle Consistency Loss](https://www.youtube.com/watch?time_continue=25&v=pPbWXmVgY0k)
	2. [Quiz](iamges/quiz_cyclegan.png)