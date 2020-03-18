# Introduction

## Lessons

1. Lesson 1: Welcome To Deep Learning
	1. [Welcome to the Deep Learning Nanodegree Program](https://www.youtube.com/watch?v=5U9tUZR3j9s&feature=emb_logo) 
	1. [Meet Your Instructors](https://www.youtube.com/watch?v=I1VodFLH5qo&feature=emb_logo)
	1. Program Structure
	```
Program Structure
The Deep Learning Nanodegree program is divided into five parts, giving you a thorough understanding of deep learning, and covering some of the major topics.
Introduction
The first part is an introduction to the program as well as a couple lessons covering tools you'll be using. You'll also get a chance to apply some deep learning models to do cool things like transferring the style of artwork to another image.
We’ll start off with a simple introduction to linear regression and machine learning. This will give you the vocabulary you need to understand recent advancements, and make clear where deep learning fits into the broader picture of machine learning techniques.
Neural Networks
In this part, you'll learn how to build a simple neural network from scratch using python. We'll cover the algorithms used to train networks such as gradient descent and backpropagation.
The first project is also available this week. In this project, you'll predict bike ridership using a simple neural network.
Multi-layer neural network with some inputs and a single output. Image from Stanford's cs231n course.
Sentiment Analysis
You'll also learn about model evaluation and validation, an important technique for training and assessing neural networks. We also have guest instructor Andrew Trask, author of Grokking Deep Learning, developing a neural network for processing text and predicting sentiment. The exercises in each chapter of his book are also available in his Github repository.
Deep Learning with PyTorch
The last lesson will be all about using the deep learning framework, PyTorch. Here, you'll learn how to use the Tensor datatype, and the foundational knowledge you'll need to define and train your own deep learning models in PyTorch!
PyTorch logo
Convolutional Networks
Convolutional networks have achieved state of the art results in computer vision. These types of networks can detect and identify objects in images. You'll learn how to build convolutional networks in PyTorch.
You'll also get the second project, where you'll build a convolutional network to classify dog breeds in pictures.
Structure of a convolutional neural network.
You'll also use convolutional networks to build an autoencoder, a network architecture used for image compression and denoising. Then, you'll use a pre-trained neural network, to classify images the network has never seen before, a technique known as transfer learning.
Recurrent Neural Networks
In this part, you’ll learn about Recurrent Neural Networks (RNNs) — a type of network architecture particularly well suited to data that forms sequences like text, music, and time series data. You'll build a recurrent neural network that can generate new text character by character.
Examples of input/output sequence types.
Natural Language Processing
Then, you'll learn about word embeddings and implement the Word2Vec model, a network that can learn about semantic relationships between words. These are used to increase the efficiency of networks when you're processing text.
You'll combine embeddings and an RNN to predict the sentiment of movie reviews, an example of common tasks in natural language processing.
In the third project, you'll use what you've learned here to generate new TV scripts from provided, existing scripts.
An example RNN structure in which an encoder represents the question: "how are you?" and a decoder generates the answer: "I am good"
Generative Adversarial Networks
Generative adversarial networks (GANs) are one of the newest and most exciting deep learning architectures, showing incredible capacity for understanding real-world data. In this part, you'll learn about and implement GANs for a variety of tasks. You'll even see how to code a CycleGAN for generating images, and learn from one of the creators of this formulation, Jun-Yan Zhu, a researcher at MIT's CSAIL.
Examples of image-to-image translation done by CycleGAN and Pix2Pix formulations.
The inventor of GANs, Ian Goodfellow, will show you how GANs work and how to implement them. Then, in the fourth project, you'll use a deep convolutional GAN to generate completely new images of human faces.
Low-res, GAN-generated images of faces.
Deploying Machine Learning Models
As more and more companies look to build AI products, there is a growing demand for engineers who are able to deploy machine learning models to global audiences. In this part, you’ll get experience deploying a model so that it can be accessed via a web app and respond to user input.
Image of a cloud service connecting data to a laptop.
You'll also learn to monitor a model using PyTorch and Amazon's SageMaker. In the fifth project, you will deploy your own PyTorch sentiment analysis model and create a gateway for accessing this model from a website.
Projects You Will Build
The five projects you'll complete in this course are perhaps the most important part of your learning journey. They give you the chance to apply what you've learned and even share your work with friends or potential employers! These projects are designed to be challenging and interesting, as such, you may not always pass on the first attempt, but, if you are enrolled in our complete program, you will get feedback from a real person; a Udacity reviewer. This reviewer will help you figure out what could be improved in your code and you can submit your code again until you pass the project.
Here are the five projects, listed for convenience:
Predicting Bike-Sharing Data
Dog Breed Classifier
Generate TV Scripts
Generate Faces
Deploy a Sentiment Analysis Model
You are also encouraged to keep a public portfolio of completed project code on a personal Github or write a blog posts about your problem-solving approach.
Deadlines
We provide deadlines for these projects to help you stay on track. You will find these deadlines posted in the classroom. The deadlines aren't mandatory, and there are no consequences for missing them. But, do try to stick to them so you complete the program in time.	
	```
	1. Prerequisites
```
Prerequisites
We've designed this program such that you only require the following prerequisite knowledge:

Required
Intermediate Python experience.
Optional
Multivariable Calculus and Linear Algebra if possible.
That being said, we've included a lot of the detailed mathematics for those of you who do want to go in depth and understand the theory behind these concepts. Such content is optional and shouldn't prevent you from doing the projects. However, it is encouraged for a theoretical understanding.
```
	1. [Getting Set Up](https://www.youtube.com/watch?v=1SuxTnuQkeE&feature=emb_logo)
1. Lesson 5: Anaconda
	1. [Introduction](https://www.youtube.com/watch?time_continue=6&v=VXukXZv7SCQ&feature=emb_logo)
	1. Installing Anaconda
	```
	Installing Anaconda
Anaconda is available for Windows, Mac OS X, and Linux. You can find the installers and installation instructions at https://www.anaconda.com/download/.
If you already have Python installed on your computer, this won't break anything. Instead, the default Python used by your scripts and programs will be the one that comes with Anaconda.
Choose the Python 3.6 version, you can install Python 2 versions later. Also, choose the 64-bit installer if you have a 64-bit operating system, otherwise go with the 32-bit installer. Go ahead and choose the appropriate version, then install it. Continue on afterwards!
After installation, you’re automatically in the default conda environment with all packages installed which you can see below. You can check out your own install by entering conda list into your terminal.
On Windows
A bunch of applications are installed along with Anaconda:
Anaconda Navigator, a GUI for managing your environments and packages
Anaconda Prompt, a terminal where you can use the command line interface to manage your environments and packages
Spyder, an IDE geared toward scientific development
To avoid errors later, it's best to update all the packages in the default environment. Open the Anaconda Prompt application. In the prompt, run the following commands:
conda upgrade conda
conda upgrade --all
and answer yes when asked if you want to install the packages. The packages that come with the initial install tend to be out of date, so updating them now will prevent future errors from out of date software.
Note: In the previous step, running conda upgrade conda should not be necessary because --all includes the conda package itself, but some users have encountered errors without it.
In the rest of this lesson, I'll be asking you to use commands in your terminal. I highly suggest you start working with Anaconda this way, then later use the GUI if you'd like.
Troubleshooting
If you are seeing the following "conda command not found" and are using ZShell, you have to do the following:
Add export PATH="/Users/username/anaconda/bin:$PATH" to your .zsh_config file.
	```
	1. Managing packages
	```
Managing Packages
Once you have Anaconda installed, managing packages is fairly straightforward. To install a package, type conda install package_name in your terminal. For example, to install numpy, type conda install numpy.
You can install multiple packages at the same time. Something like conda install numpy scipy pandas will install all those packages simultaneously. It's also possible to specify which version of a package you want by adding the version number such as conda install numpy=1.10.
Conda also automatically installs dependencies for you. For example scipy depends on numpy, it uses and requires numpy. If you install just scipy (conda install scipy), Conda will also install numpy if it isn't already installed.
Most of the commands are pretty intuitive. To uninstall, use conda remove package_name. To update a package conda update package_name. If you want to update all packages in an environment, which is often useful, use conda update --all. And finally, to list installed packages, it's conda list which you've seen before.
If you don't know the exact name of the package you're looking for, you can try searching with conda search *search_term*. For example, I know I want to install Beautiful Soup, but I'm not sure of the exact package name. So, I try conda search *beautifulsoup*. Note that your shell might expand the wildcard * before running the conda command. To fix this, wrap the search string in single or double quotes like conda search '*beautifulsoup*'.
It returns a list of the Beautiful Soup packages available with the appropriate package name, beautifulsoup4.
QUIZ QUESTION
Which of these commands would you use to install the packages numpy and pandas with conda? (More than one might be correct - select all that apply.)
conda install pandas
conda install numpy pandas	
	```
	1. Managing environments
	```
	Managing environments
As I mentioned before, conda can be used to create environments to isolate your projects. To create an environment, use conda create -n env_name list of packages in your terminal. Here -n env_name sets the name of your environment (-n for name) and list of packages is the list of packages you want installed in the environment. For example, to create an environment named my_env and install numpy in it, type conda create -n my_env numpy.
When creating an environment, you can specify which version of Python to install in the environment. This is useful when you're working with code in both Python 2.x and Python 3.x. To create an environment with a specific Python version, do something like conda create -n py3 python=3 or conda create -n py2 python=2. I actually have both of these environments on my personal computer. I use them as general environments not tied to any specific project, but rather for general work with each Python version easily accessible. These commands will install the most recent version of Python 3 and 2, respectively. To install a specific version, use conda create -n py python=3.3 for Python 3.3.
Entering an environment
Once you have an environment created, use conda activate my_env to enter it.
When you're in the environment, you'll see the environment name in the terminal prompt. Something like (my_env) ~ $. The environment has only a few packages installed by default, plus the ones you installed when creating it. You can check this out with conda list. Installing packages in the environment is the same as before: conda install package_name. Only this time, the specific packages you install will only be available when you're in the environment. To leave the environment, type source deactivate (on OSX/Linux). On Windows, use deactivate.
QUIZ QUESTION
What command would you use to create an environment named data installed with Python 3.6, numpy, and pandas?
conda create -n data python=3.6 numpy pandas
	```	
	1. More environment actions
	```
	Saving and loading environments
A really useful feature is sharing environments so others can install all the packages used in your code, with the correct versions. You can save the packages to a YAML file with conda env export > environment.yaml. The first part conda env export writes out all the packages in the environment, including the Python version.
Exported environment printed to the terminal
Above you can see the name of the environment and all the dependencies (along with versions) are listed. The second part of the export command, > environment.yaml writes the exported text to a YAML file environment.yaml. This file can now be shared and others will be able to create the same environment you used for the project.
To create an environment from an environment file use conda env create -f environment.yaml. This will create a new environment with the same name listed in environment.yaml.
Listing environments
If you forget what your environments are named (happens to me sometimes), use conda env list to list out all the environments you've created. You should see a list of environments, there will be an asterisk next to the environment you're currently in. The default environment, the environment used when you aren't in one, is called root.
Removing environments
If there are environments you don't use anymore, conda env remove -n env_name will remove the specified environment (here, named env_name).
	```
	1. Best practices
	```
	Best practices
Using environments
One thing that’s helped me tremendously is having separate environments for Python 2 and Python 3. I used conda create -n py2 python=2 and conda create -n py3 python=3 to create two separate environments, py2 and py3. Now I have a general use environment for each Python version. In each of those environments, I've installed most of the standard data science packages (numpy, scipy, pandas, etc.). Remember that when you set up an environment initially, you'll only start with the standard packages and whatever packages you specify in your conda create statement.
I’ve also found it useful to create environments for each project I’m working on. It works great for non-data related projects too like web apps with Flask. For example, I have an environment for my personal blog using Pelican.
Sharing environments
When sharing your code on GitHub, it's good practice to make an environment file and include it in the repository. This will make it easier for people to install all the dependencies for your code. I also usually include a pip requirements.txt file using pip freeze (learn more here) for people not using conda.
More to learn
To learn more about conda and how it fits in the Python ecosystem, check out this article by Jake Vanderplas: Conda myths and misconceptions. And here's the conda documentation you can reference later, and a link to a cheatsheet to help you basic conda commands.
	```
1. Lesson 6: Applying Deep Learning
	1. Style Transfer
```
Style Transfer
As an example of the kind of things you'll be building with deep learning models, here is a really fun project, fast style transfer. Style transfer allows you to take famous paintings, and recreate your own images in their styles! The network learns the underlying techniques of those paintings and figures out how to apply them on its own. This model was trained on the styles of famous paintings and is able to transfer those styles to other images and even videos!

I used it to style my cat Chihiro in the style of Hokusai's The Great Wave Off Kanagawa.


To try it out yourself, you can find the code in the fast-style-transfer GitHub repo. Either use git to clone the repository, or you can download the whole thing as a Zip archive and extract it.

The network has been trained on a few different styles (here) and saved into checkpoint files. Checkpoint files contain all the information about the trained network to apply styles to new images.

Dependencies
The easiest way to install all the packages needed to run this code is with Anaconda. Anaconda comes with Conda, a package and environment manager built specifically for data science. Install the Python 3 version of Anaconda appropriate for your operating system.

If you haven't used Conda before, please quickly run through the Anaconda lesson first.

You'll need to install Python 3, Tensorflow, Pillow, and SciPy, and moviepy. The process should be the same whether you're using a Mac, Windows, or Linux. After installing Anaconda, open your command prompt. In there, enter these commands line by line:

conda create -n style-transfer python=3
conda activate style-transfer
conda install tensorflow scipy pillow
pip install moviepy
python -c "import imageio; imageio.plugins.ffmpeg.download()"
Note: If you get an error on the last command that ends in RuntimeError: imageio.ffmpeg.download() has been deprecated. Use 'pip install imageio-ffmpeg' instead.' just run the command pip install imageio-ffmpeg. You may need to restart the terminal and reactivate the environment for the command to complete.

Let’s take a quick look at what these commands do. The first line in both sets of instructions, creates a new environment with Python 3. This environment will hold all the packages you need for the style transfer code. The next line enters the environment. Next, we install TensorFlow, SciPy, Pillow (which is an image processing library), and moviepy. The last line here installs ffmpeg, an application for converting images and videos.

Transferring styles
Download the Zip archive from the fast-style-transfer repository and extract it. You can download it by clicking on the bright green button on the right.
Download the Rain Princess checkpoint from here. Put it in the fast-style-transfer folder. A checkpoint file is a model that already has tuned parameters. By using this checkpoint file, we won't need to train the model and can get straight to applying it.
Copy the image you want to style into the fast-style-transfer folder.
Enter the Conda environment you created above, if you aren't still in it.
Finally, in your terminal, navigate to the fast-style-transfer folder and enter

python evaluate.py --checkpoint ./rain-princess.ckpt --in-path <path_to_input_file> --out-path ./output_image.jpg
Note: Your checkpoint file might be named rain_princess.ckpt, notice the underscore, it's not the dash from above.

You can get more checkpoint files at the bottom of this page. Try them all!

Feel free to train the network on your own images, you can find instructions in the repository (although it does take some powerful hardware).

Note: Be careful with the size of the input image. The style transfer can take quite a while to run on larger images.

Style Transfer Checklist
Task List




The checkpoints were trained on the following paintings:

Rain Princesss, by Leonid Afremov
La Muse, by Pablo Picasso
Udnie by Francis Picabia
Scream, by Edvard Munch
The Great Wave off Kanagawa, by Hokusai
The Shipwreck of the Minotaur, by J.M.W. Turner
Supporting Materials
 [Rain Princess checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/587d1865_rain-princess/rain-princess.ckpt)
 [La Muse checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/588aa800_la-muse/la-muse.ckpt)
 [Udnie checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/588aa846_udnie/udnie.ckpt)
 [Scream checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/588aa883_scream/scream.ckpt)
 [Wave checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/588aa89d_wave/wave.ckpt)
 [Wreck checkpoint](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/January/588aa8b6_wreck/wreck.ckpt)
```
![chi-waves](chi-waves.png)
	1. [DeepTraffic](https://www.youtube.com/watch?v=az5ElmV4DhY&feature=emb_logo)
	1. Flappy Bird
	```
	Flappy Bird
In this example, you'll get to see a deep learning agent playing Flappy Bird! You have the option to train the agent yourself, but for now let's just start with the pre-trained network given by the author. Note that the following agent is able to play without being told any information about the structure of the game or its rules. It automatically discovers the rules of the game by finding out how it did on each iteration.
We will be following this repository by Yenchen Lin.
Instructions
Install miniconda or anaconda if you have not already.
Create an environment for flappybird
Mac/Linux: conda create --name=flappybird python=2.7
Windows: conda create --name=flappybird python=3.5
Enter your conda environment: conda activate flappybird
conda install opencv
If you encounter an error here, you may try an alternate download path and instead type conda install --channel https://conda.anaconda.org/menpo opencv3
pip install pygame
pip install tensorflow==0.12
git clone https://github.com/yenchenlin/DeepLearningFlappyBird.git
If you don't have git installed, you can download and extract the zip archive directly from the repository
cd DeepLearningFlappyBird
If you downloaded the archive, you will need to navigate to the extracted folder DeepLearningFlappyBird-master instead
python deep_q_network.py
If all went correctly, you should be seeing a deep learning based agent play Flappy Bird! The repository contains instructions for training your own agent if you're interested!
You can also, typically, force-quit out of the game by returning to your terminal window and typing Command or Ctrl + C.
	```
	1. Books to Read
```
We believe that you learn best when you are exposed to multiple perspectives on the same idea. As such, we recommend checking out a few of the books below to get an added perspective on Deep Learning.
Grokking Deep Learning by Andrew Trask. Use our exclusive discount code traskud17 for 40% off. This provides a very gentle introduction to Deep Learning and covers the intuition more than the theory.
Neural Networks And Deep Learning by Michael Nielsen. This book is more rigorous than Grokking Deep Learning and includes a lot of fun, interactive visualizations to play with.
The Deep Learning Textbook from Ian Goodfellow, Yoshua Bengio, and Aaron Courville. This online book contains a lot of material and is the most rigorous of the three books suggested.
```
1. Lesson 7: Jupyter Notebook
	1. [What are Jupyter notebooks?](https://www.youtube.com/watch?v=qiYDWFLyXvg&feature=emb_logo)
	1. Installing Jupyter Notebook
```
Installing Jupyter Notebook
By far the easiest way to install Jupyter is with Anaconda. Jupyter notebooks automatically come with the distribution. You'll be able to use notebooks from the default environment.

To install Jupyter notebooks in a conda environment, use conda install jupyter notebook.

Jupyter notebooks are also available through pip with pip install jupyter notebook.
```
	1. Launching the notebook server
```
Launching the notebook server
To start a notebook server, enter jupyter notebook in your terminal or console. This will start the server in the directory you ran the command in. That means any notebook files will be saved in that directory. Typically you'd want to start the server in the directory where your notebooks live. However, you can navigate through your file system to where the notebooks are.

When you run the command (try it yourself!), the server home should open in your browser. By default, the notebook server runs at http://localhost:8888. If you aren't familiar with this, localhost means your computer and 8888 is the port the server is communicating on. As long as the server is still running, you can always come back to it by going to http://localhost:8888 in your browser.

If you start another server, it'll try to use port 8888, but since it is occupied, the new server will run on port 8889. Then, you'd connect to it at http://localhost:8889. Every additional notebook server will increment the port number like this.

If you tried starting your own server, it should look something like this:


You might see some files and folders in the list here, it depends on where you started the server from.

Over on the right, you can click on "New" to create a new notebook, text file, folder, or terminal. The list under "Notebooks" shows the kernels you have installed. Here I'm running the server in a Python 3 environment, so I have a Python 3 kernel available. You might see Python 2 here. I've also installed kernels for Scala 2.10 and 2.11 which you see in the list.

The tabs at the top show Files, Running, and Cluster. Files shows all the files and folders in the current directory. Clicking on the Running tab will list all the currently running notebooks. From there you can manage them.

Clusters previously was where you'd create multiple kernels for use in parallel computing. Now that's been taken over by ipyparallel so there isn't much to do there.

You should consider installing Notebook Conda to help manage your environments. Run the following command:

conda install nb_conda

Then if you run the notebook server from a conda environment, you'll also have access to the "Conda" tab shown below. Here you can manage your environments from within Jupyter. You can create new environments, install packages, update packages, export environments and more.


conda tab in Jupyter

Additionally, with nb_conda installed you will be able to access any of your conda environments when choosing a kernel. For example, the image below shows an example of creating a new notebook on a machine with several different conda environments:


conda environments in Jupyter

Shutting down Jupyter
You can shutdown individual notebooks by marking the checkbox next to the notebook on the server home and clicking "Shutdown." Make sure you've saved your work before you do this though! Any changes since the last time you saved will be lost. You'll also need to rerun the code the next time you run the notebook.


You can shutdown the entire server by pressing control + C twice in the terminal. Again, this will immediately shutdown all the running notebooks, so make sure your work is saved!

```
	1. Notebook interface
```
Notebook interface
When you create a new notebook, you should see something like this:


Feel free to try this yourself and poke around a bit.

You’ll see a little box outlined in green. This is called a cell. Cells are where you write and run your code. You can also change it to render Markdown, a popular formatting syntax for writing web content. I'll cover Markdown in more detail later. In the toolbar, click “Code” to change it to Markdown and back. The little play button runs the cell, and the up and down arrows move cells up and down.

When you run a code cell, the output is displayed below the cell. The cell also gets numbered, you see In [1]: on the left. This lets you know the code was run and the order if you run multiple cells. Running the cell in Markdown mode renders the Markdown as text.

The tool bar
Elsewhere on the tool bar, starting from the left:

The anachronistic symbol for "save," the floppy disk. Saves the notebook!
The + button creates a new cell
Then, buttons to cut, copy, and paste cells.
Run, stop, restart the kernel
Cell type: code, Markdown, raw text, and header
Command palette (see next)
Cell toolbar, gives various options for cells such as using them as slides
Command palette
The little keyboard is the command palette. This will bring up a panel with a search bar where you can search for various commands. This is really helpful for speeding up your workflow as you don't need to search around in the menus with your mouse. Just open the command palette and type in what you want to do. For instance, if you want to merge two cells:

More things
At the top you see the title. Click on this to rename the notebook.

Over on the right is the kernel type (Python 3 in my case) and next to it, a little circle. When the kernel is running a cell, it'll fill in. For most operations which run quickly, it won't fill in. It's a little indicator to let you know longer running code is actually running.

Along with the save button in the toolbar, notebooks are automatically saved periodically. The most recent save is noted to the right of the title. You can save manually with the save button, or by pressing escape then s on your keyboard. The escape key changes to command mode and s is the shortcut for "save." I'll cover command mode and keyboard shortcuts later.

In the "File" menu, you can download the notebook in multiple formats. You'll often want to download it as an HTML file to share with others who aren't using Jupyter. Also, you can download the notebook as a normal Python file where all the code will run like normal. The Markdown and reST formats are great for using notebooks in blogs or documentation.


```
	1. Code cells
```
Code cells
Most of your work in notebooks will be done in code cells. This is where you write your code and it gets executed. In code cells you can write any code, assigning variables, defining functions and classes, importing packages, and more. Any code executed in one cell is available in all other cells.

To give you some practice, I created a notebook you can work through. Download the notebook Working With Code Cells below then run it from your own notebook server. (In your terminal, change to the directory with the notebook file, then enter jupyter notebook) Your browser might try to open the notebook file without downloading it. If that happens, right click on the link then choose "Save Link As..."

Supporting Materials
[Working With Code Cells](http://video.udacity-data.com.s3.amazonaws.com/topher/2016/December/58474202_working-with-code-cells/working-with-code-cells.ipynb)
```
	1. Markdown cells
```
Markdown cells
As mentioned before, cells can also be used for text written in Markdown. Markdown is a formatting syntax that allows you to include links, style text as bold or italicized, and format code. As with code cells, you press Shift + Enter or Control + Enter to run the Markdown cell, where it will render the Markdown to formatted text. Including text allows you to write a narrative alongside your code, as well as documenting your code and the thoughts that went into it.

You can find the documentation here, but I'll provide a short primer.

Headers
You can write headers using the pound/hash/octothorpe symbol # placed before the text. One # renders as an h1 header, two #s is an h2, and so on. Looks like this:

# Header 1
## Header 2
### Header 3
renders as

Header 1
Header 2
Header 3
Links
Linking in Markdown is done by enclosing text in square brackets and the URL in parentheses, like this [Udacity's home page](https://www.udacity.com) for a link to Udacity's home page.

Emphasis
You can add emphasis through bold or italics with asterisks or underscores (* or _). For italics, wrap the text in one asterisk or underscore, _gelato_ or *gelato* renders as gelato.

Bold text uses two symbols, **aardvark** or __aardvark__ looks like aardvark.

Either asterisks or underscores are fine as long as you use the same symbol on both sides of the text.

Code
There are two different ways to display code, inline with text and as a code block separated from the text. To format inline code, wrap the text in backticks. For example, `string.punctuation` renders as string.punctuation.

To create a code block, start a new line and wrap the text in three backticks

```
import requests
response = requests.get('https://www.udacity.com')
```
or indent each line of the code block with four spaces.

import requests
response = requests.get('https://www.udacity.com')
Math expressions
You can create math expressions in Markdown cells using LaTeX symbols. Notebooks use MathJax to render the LaTeX symbols as math symbols. To start math mode, wrap the LaTeX in dollar signs $y = mx + b$ for inline math. For a math block, use double dollar signs,

$$
y = \frac{a}{b+c}
$$
This is a really useful feature, so if you don't have experience with LaTeX, here is a tutorial on using it to create math expressions.

Wrapping up
Here's a cheatsheet you can use as a reference for writing Markdown. My advice is to make use of the Markdown cells. Your notebooks will be much more readable compared to a bunch of code blocks.
```
	1. Keyboard shortcuts
```
Notebooks come with a bunch of keyboard shortcuts that let you use your keyboard to interact with the cells, instead of using the mouse and toolbars. They take a bit of time to get used to, but when you're proficient with the shortcuts you'll be much faster at working in notebooks. To learn more about the shortcuts and get practice using them, download the notebook Keyboard Shortcuts below. Again, your browser might try to open it, but you want to save it to your computer. Right click on the link, then choose "Save Link As..."

Supporting Materials
[Keyboard-Shortcuts](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/April/58e412d0_keyboard-shortcuts/keyboard-shortcuts.ipynb)
```
	1. Magic keywords
```
Magic keywords
Magic keywords are special commands you can run in cells that let you control the notebook itself or perform system calls such as changing directories. For example, you can set up matplotlib to work interactively in the notebook with %matplotlib.

Magic commands are preceded with one or two percent signs (% or %%) for line magics and cell magics, respectively. Line magics apply only to the line the magic command is written on, while cell magics apply to the whole cell.

NOTE: These magic keywords are specific to the normal Python kernel. If you are using other kernels, these most likely won't work.

Timing code
At some point, you'll probably spend some effort optimizing code to run faster. Timing how quickly your code runs is essential for this optimization. You can use the timeit magic command to time how long it takes for a function to run, like so:


If you want to time how long it takes for a whole cell to run, you’d use %%timeit like so:


Embedding visualizations in notebooks
As mentioned before, notebooks let you embed images along with text and code. This is most useful when you’re using matplotlib or other plotting packages to create visualizations. You can use %matplotlib to set up matplotlib for interactive use in the notebook. By default figures will render in their own window. However, you can pass arguments to the command to select a specific "backend", the software that renders the image. To render figures directly in the notebook, you should use the inline backend with the command %matplotlib inline.

Tip: On higher resolution screens such as Retina displays, the default images in notebooks can look blurry. Use %config InlineBackend.figure_format = 'retina' after %matplotlib inline to render higher resolution images.


Example figure in a notebook

Debugging in the Notebook
With the Python kernel, you can turn on the interactive debugger using the magic command %pdb. When you cause an error, you'll be able to inspect the variables in the current namespace.


Debugging in a notebook

Above you can see I tried to sum up a string which gives an error. The debugger raises the error and provides a prompt for inspecting your code.

Read more about pdb in the documentation. To quit the debugger, simply enter q in the prompt.

More reading
There are a whole bunch of other magic commands, I just touched on a few of the ones you'll use the most often. To learn more about them, here's the [list](http://ipython.readthedocs.io/en/stable/interactive/magics.html) of all available magic commands.
```
	1. Converting notebooks
```
Converting notebooks
Notebooks are just big JSON files with the extension .ipynb.


Notebook file opened in a text editor shows JSON data

Since notebooks are JSON, it is simple to convert them to other formats. Jupyter comes with a utility called nbconvert for converting to HTML, Markdown, slideshows, etc.

For example, to convert a notebook to an HTML file, in your terminal use

jupyter nbconvert --to html notebook.ipynb
Converting to HTML is useful for sharing your notebooks with others who aren't using notebooks. Markdown is great for including a notebook in blogs and other text editors that accept Markdown formatting.


As always, learn more about nbconvert from the documentation.
```
	1. Creating a slideshow
```
Creating a slideshow
Create slideshows from notebooks is one of my favorite features. You can see an [example](http://nbviewer.jupyter.org/format/slides/github/jorisvandenbossche/2015-PyDataParis/blob/master/pandas_introduction.ipynb#/) of a slideshow here introducing pandas for working with data.

The slides are created in notebooks like normal, but you'll need to designate which cells are slides and the type of slide the cell will be. In the menu bar, click View > Cell Toolbar > Slideshow to bring up the slide cell menu on each cell.


Turning on Slideshow toolbars for cells

This will show a menu dropdown on each cell that lets you choose how the cell shows up in the slideshow.


Choose slide type

Slides are full slides that you move through left to right. Sub-slides show up in the slideshow by pressing up or down. Fragments are hidden at first, then appear with a button press. You can skip cells in the slideshow with Skip and Notes leaves the cell as speaker notes.

Running the slideshow
To create the slideshow from the notebook file, you'll need to use nbconvert:

    jupyter nbconvert notebook.ipynb --to slides
This just converts the notebook to the necessary files for the slideshow, but you need to serve it with an HTTP server to actually see the presentation.

To convert it and immediately see it, use

jupyter nbconvert notebook.ipynb --to slides --post serve
This will open up the slideshow in your browser so you can present it.
```
1. Lesson 8: Numpy
	1. [Data Dimensions](https://www.youtube.com/watch?v=F4NSv776X0c&feature=emb_logo)
	1. [Element-wise Matrix Operations](https://www.youtube.com/watch?v=vjUykZyzko4&feature=emb_logo)
	1. [Matrix Multiplication: Part 1](https://www.youtube.com/watch?v=JRoCFQRP4B0&feature=emb_logo)
	1. [Matrix Multiplication: Part 2](https://www.youtube.com/watch?v=8jtk8BzBdj8&feature=emb_logo)
	1. [Matrix Transposes](https://www.youtube.com/watch?v=NVK5xCY3CZE&feature=emb_logo)