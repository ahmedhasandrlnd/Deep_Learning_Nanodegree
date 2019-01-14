# Lesson 3: Deploying and using a Model

## Concepts

1. [Deploying a Model in SageMaker](https://www.youtube.com/watch?v=g_GYZpcVcFE)
	> Deploying model means create an endpoint which is basically a way to allow a model and an application to communicate. An application, such as a web app, will be responsible for accepting user input data, and through an endpoint we can send that data to our model, which will produce predictions that can be sent back to our application!
1. [Boston Housing Example - Deploying the Model](https://www.youtube.com/watch?v=0PBsV-SzSlo)
	> Using the high level approach makes deploying a trained model pretty straightforward. All we need to do is call the deploy method and SageMaker takes care of the rest.

	> Similarly, sending data to the deployed endpoint and capturing the resulting inference is easy too as SageMaker wraps everything up into the predict method, provided we make sure that our data is serialized correctly. In our case, serializing means converting the data structure we wish to send to our endpoint into a string, something that can be transferred using HTTP.
1. [Boston Housing In-Depth - Deploying the Model](https://www.youtube.com/watch?v=1lzWAzypJ9k)
1. [Deploying and Using a Sentiment Analysis Model](https://www.youtube.com/watch?v=r7XVQEojRKk)