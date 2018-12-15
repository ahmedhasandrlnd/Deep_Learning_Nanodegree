# Implementation of RNN & LSTM 

## Concepts

1. [Implementing RNNs](https://www.youtube.com/watch?time_continue=5&v=BHoiwB61ays)
> Two Challenges
>* Pre-process sequential data
>* Represent Memory
1. [Time-Series Prediction](https://www.youtube.com/watch?time_continue=4&v=xV5jHLFfJbQ)
>This video is a walkthrough of code that you can find in our public Github repository, if you navigate to recurrent-neural-networks > time-series and the Simple_RNN.ipynb notebook. Feel free to go through this code on your own, locally.
1. [Training & Memory](https://www.youtube.com/watch?time_continue=7&v=sx7T_KP5v9I)
>[Quiz](images/Quiz_implementation_lstm.png)
1. [Character-wise RNNs](https://www.youtube.com/watch?v=dXl3eWCGLdU)
1. [Sequence Batching](https://www.youtube.com/watch?v=Z4OiyU0Cldg)
1. Pre-Notebook: Character-Level RNN
> Clone the repo from Github and open the notebook Character_Level_RNN_Exercise.ipynb in the recurrent-neural-networks > char-rnn folder. You can either download the repository with git clone https://github.com/udacity/deep-learning-v2-pytorch.git
1. Notebook: Character-Level RNN
1. [Implementing a Char-RNN](https://www.youtube.com/watch?v=MMtgZXzFB10)
> Typo: Above you may see the title, Chararacter_Level_RNN_Exercise. This is a mistake on my part and the in-classroom notebooks have been updated with the correct spelling.
Know that the code is correct even if the title has a typo :)
1. [Batching Data, Solution](https://www.youtube.com/watch?v=9Eg0wf3eW-k)
1. [Defining the Model](https://www.youtube.com/watch?v=_LWzyqq4hCY)
> Contiguous variables
If you are stacking up multiple LSTM outputs, it may be necessary to use .contiguous() to reshape the output. The notebook and Github repo code has been updated to include this use case in the forward function of the model:
`#stack up LSTM outputs
out = out.contiguous().view(-1, self.n_hidden)`
1. [Char-RNN, Solution](https://www.youtube.com/watch?v=ed33qePHrJM)
1. [Making Predictions](https://www.youtube.com/watch?time_continue=9&v=BhrpV3kwATo)
> [sketch-rnn by Magenta](sketch-rnn by Magenta)







