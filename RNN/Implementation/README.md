# Implementation of RNN & LSTM 

## Concepts

* [Implementing RNNs](https://www.youtube.com/watch?time_continue=5&v=BHoiwB61ays)
	* Two Challenges
		* Pre-process sequential data
		* Represent Memory

* [Time-Series Prediction](https://www.youtube.com/watch?time_continue=4&v=xV5jHLFfJbQ)
>This video is a walkthrough of code that you can find in our public Github repository, if you navigate to recurrent-neural-networks > time-series and the Simple_RNN.ipynb notebook. Feel free to go through this code on your own, locally.
* [Training & Memory](https://www.youtube.com/watch?time_continue=7&v=sx7T_KP5v9I)
	* [Quiz](images/Quiz_implementation_lstm.png)
* [Character-wise RNNs](https://www.youtube.com/watch?v=dXl3eWCGLdU)
* [Sequence Batching](https://www.youtube.com/watch?v=Z4OiyU0Cldg)
* Pre-Notebook: Character-Level RNN
> Clone the repo from Github and open the notebook Character_Level_RNN_Exercise.ipynb in the recurrent-neural-networks > char-rnn folder. You can either download the repository with git clone https://github.com/udacity/deep-learning-v2-pytorch.git
* Notebook: Character-Level RNN
* [Implementing a Char-RNN](https://www.youtube.com/watch?v=MMtgZXzFB10)
> Typo: Above you may see the title, Chararacter_Level_RNN_Exercise. This is a mistake on my part and the in-classroom notebooks have been updated with the correct spelling.
Know that the code is correct even if the title has a typo :)
* [Batching Data, Solution](https://www.youtube.com/watch?v=9Eg0wf3eW-k)
* [Defining the Model](https://www.youtube.com/watch?v=_LWzyqq4hCY)
	* Contiguous variables
If you are stacking up multiple LSTM outputs, it may be necessary to use .contiguous() to reshape the output. The notebook and Github repo code has been updated to include this use case in the forward function of the model:

	```
 	#stack up LSTM outputs
	out = out.contiguous().view(-1, self.n_hidden)
	```
* [Char-RNN, Solution](https://www.youtube.com/watch?v=ed33qePHrJM)
* [Making Predictions](https://www.youtube.com/watch?time_continue=9&v=BhrpV3kwATo)
	* [sketch-rnn by Magenta](https://magenta.tensorflow.org/assets/sketch_rnn_demo/index.html)







