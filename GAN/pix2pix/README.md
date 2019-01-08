# Lesson 3: Pix2Pix and CycleGAN

## Concepts

1. [Introducing Jun-Yan Zhu](https://www.youtube.com/watch?time_continue=3&v=l8sCN1rMt6E)
1. [Image to Image Translation](https://www.youtube.com/watch?time_continue=2&v=f-WnvKQd10k)
	1. Ian Goodfellow's [original paper on GANs](http://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf)
	1. Face swap with [CycleGAN Face-off](https://arxiv.org/pdf/1712.03451.pdf)
1. [Designing Loss Functions](https://www.youtube.com/watch?time_continue=4&v=YL1kKWHr7Gc)
	> The objective function we've used the most in this program is cross entropy loss, which is a negative log loss applied to the output of a softmax layer. For a binary classification problem, as in real or fake image data, we can calculate the binary cross entropy loss as:

-[y\log(\hat{y}) +(1-y) \log (1-\hat{y})] −[ylog( 
y
^
​	 )+(1−y)log(1− 
y
^
​	 )]

In other words, a sum of two log losses!