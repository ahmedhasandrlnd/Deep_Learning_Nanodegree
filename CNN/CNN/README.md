# Lesson 1: CNN

## Concepts
1. [Introduction](https://www.youtube.com/watch?v=38ExGpdyvJI&feature=emb_logo)
1. [Applications of CNNs](https://www.youtube.com/watch?v=HrYNL_1SV2Y&feature=emb_logo)
```
Optional Resources
Read about the [WaveNet](https://deepmind.com/blog/wavenet-generative-model-raw-audio/) model.

Why train an A.I. to talk, when you can train it to sing ;)? In April 2017, researchers used a variant of the WaveNet model to generate songs. The original paper and demo can be found [here](http://www.creativeai.net/posts/W2C3baXvf2yJSLbY6/a-neural-parametric-singing-synthesizer).
Learn about CNNs for [text classification](http://www.wildml.com/2015/12/implementing-a-cnn-for-text-classification-in-tensorflow/).

You might like to sign up for the author's Deep Learning [Newsletter](https://www.getrevue.co/profile/wildml)!
Read about Facebook's [novel CNN approach](https://code.facebook.com/posts/1978007565818999/a-novel-approach-to-neural-machine-translation/) for language translation that achieves state-of-the-art accuracy at nine times the speed of RNN models.

Play [Atari games](https://deepmind.com/research/dqn/) with a CNN and reinforcement learning. You can [download](https://sites.google.com/a/deepmind.com/dqn/) the code that comes with this paper.

If you would like to play around with some beginner code (for deep reinforcement learning), you're encouraged to check out Andrej Karpathy's [post](http://karpathy.github.io/2016/05/31/rl/).
Play [pictionary](https://quickdraw.withgoogle.com/#) with a CNN!

Also check out all of the other cool implementations on the [A.I. Experiments](https://aiexperiments.withgoogle.com/) website. Be sure not to miss [AutoDraw](https://www.autodraw.com/)!
Read more about [AlphaGo](https://deepmind.com/research/alphago/).

Check out this [article](https://www.technologyreview.com/s/604273/finding-solace-in-defeat-by-artificial-intelligence/?set=604287), which asks the question: If mastering Go “requires human intuition,” what is it like to have a piece of one’s humanity challenged?
Check out these really cool videos with drones that are powered by CNNs.

Here's an interview with a startup - [Intelligent Flying Machines (IFM)](https://www.youtube.com/watch?v=AMDiR61f86Y).
Outdoor autonomous navigation is typically accomplished through the use of the [global positioning system (GPS)](http://www.droneomega.com/gps-drone-navigation-works/), but here's a demo with a CNN-powered [autonomous drone](https://www.youtube.com/watch?v=wSFYOw4VIYY).
If you're excited about using CNNs in self-driving cars, you're encouraged to check out:

our Self-Driving Car Engineer Nanodegree, where we classify signs in the [German Traffic Sign dataset](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset) in this [project](https://github.com/udacity/CarND-Traffic-Sign-Classifier-Project).
our Machine Learning Engineer Nanodegree, where we classify house numbers from the [Street View House Numbers dataset](http://ufldl.stanford.edu/housenumbers/) in this [project](https://github.com/udacity/machine-learning/tree/master/projects/digit_recognition).
this [series of blog posts](https://pythonprogramming.net/game-frames-open-cv-python-plays-gta-v/) that details how to train a CNN in Python to produce a self-driving A.I. to play Grand Theft Auto V.
Check out some additional applications not mentioned in the video.

Some of the world's most famous paintings have been [turned into 3D](http://www.businessinsider.com/3d-printed-works-of-art-for-the-blind-2016-1) for the visually impaired. Although the article does not mention how this was done, we note that it is possible to use a CNN to [predict depth](https://www.cs.nyu.edu/~deigen/depth/) from a single image.
Check out [this research](https://research.googleblog.com/2017/03/assisting-pathologists-in-detecting.html) that uses CNNs to localize breast cancer.
CNNs are used to [save endangered species](https://blogs.nvidia.com/blog/2016/11/04/saving-endangered-species/?adbsc=social_20170303_70517416)!
An app called [FaceApp](http://www.digitaltrends.com/photography/faceapp-neural-net-image-editing/) uses a CNN to make you smile in a picture or change genders.
```
1. [Lesson Outline](https://www.youtube.com/watch?v=77LzWE1qQrc&feature=emb_logo)
![Q](q1.JPG)
1. [MNIST Dataset](https://www.youtube.com/watch?v=a7bvIGZpcnk&feature=emb_logo)
	> The MNIST database is arguably the most famous database in the field of deep learning! Check out [this figure](https://www.kaggle.com/benhamner/popular-datasets-over-time) that shows datasets referenced over time in [NIPS](https://nips.cc/) papers.
1. [How Computers Interpret Images](https://www.youtube.com/watch?v=mEPfoM68Fx4&feature=emb_logo)
```
Normalizing image inputs
Data normalization is an important pre-processing step. It ensures that each input (each pixel value, in this case) comes from a standard distribution. That is, the range of pixel values in one input image are the same as the range in another image. This standardization makes our model train and reach a minimum error, faster!

Data normalization is typically done by subtracting the mean (the average of all pixel values) from each pixel, and then dividing the result by the standard deviation of all the pixel values. Sometimes you'll see an approximation here, where we use a mean and standard deviation of 0.5 to center the pixel values. [Read more about the Normalize transformation in PyTorch](https://pytorch.org/docs/stable/torchvision/transforms.html#transforms-on-torch-tensor).

The distribution of such data should resemble a [Gaussian function](http://mathworld.wolfram.com/GaussianFunction.html) centered at zero. For image inputs we need the pixel numbers to be positive, so we often choose to scale the data in a normalized range [0,1].
```
1. [MLP Structure & Class Scores](https://www.youtube.com/watch?v=fP0Odiai8sk&feature=emb_logo)
1. [Do Your Research](https://www.youtube.com/watch?v=CR4JeAn1fgk&feature=emb_logo)
1. [Loss & Optimization](https://www.youtube.com/watch?v=BmPDtSXv18w&feature=emb_logo)
1. [Defining a Network in PyTorch](https://www.youtube.com/watch?time_continue=2&v=9gvaQvyfLfY&feature=emb_logo)
![Q](q2.JPG)
1. [Training the Network](https://www.youtube.com/watch?time_continue=1&v=904bfqibcCw&feature=emb_logo)
![Q](q3.JPG)
1. Pre-Notebook: MLP Classification, Exercise
![Q](q4.JPG)
1. [One Solution](https://www.youtube.com/watch?v=7q37WPjQhDA&feature=emb_logo)
![Q](q5.JPG)
Check out the [first research paper](https://www.cs.toronto.edu/~hinton/absps/JMLRdropout.pdf) to propose dropout as a technique for overfitting.
If you'd like more information on activation functions, check out this [website](http://cs231n.github.io/neural-networks-1/#actfun).
1. [Model Validation](https://www.youtube.com/watch?v=b5934VsV3SA&feature=emb_logo)
1. [Validation Loss](https://www.youtube.com/watch?v=uGPP_-pbBsc&feature=emb_logo)
![Q](q6.JPG)
1. [Image Classification Steps](https://www.youtube.com/watch?v=UHFBnitKraA&feature=emb_logo)
1. [MLPs vs CNNs](https://www.youtube.com/watch?v=Q7CR3cCOtJQ&feature=emb_logo)
Check out the performance of [other classifiers](http://yann.lecun.com/exdb/mnist/).
1. [Local Connectivity](https://www.youtube.com/watch?v=z9wiDg0w-Dc&feature=emb_logo)
1. [Filters and the Convolutional Layer](https://www.youtube.com/watch?v=x_dhnhUzFNo&feature=emb_logo)
1. [Filters & Edges](https://www.youtube.com/watch?v=hfqNqcEU6uI&feature=emb_logo)
```
Filters
To detect changes in intensity in an image, you’ll be using and creating specific image filters that look at groups of pixels and react to alternating patterns of dark/light pixels. These filters produce an output that shows edges of objects and differing textures.

So, let’s take a closer look at these filters and see when they’re useful in processing images and identifying traits of interest.
```