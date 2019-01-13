# Lesson 2: Building a Model using SageMaker

## Concepts

1. [Introduction to Amazon SageMaker](https://www.youtube.com/watch?v=nJCc4_9-iAQ)
	> 1. Notebook: explore and process data
	> 1. Apllication Programming Interface: simplifies modeling and deployment steps.It is collection of tools for training process and inference process.

	![training](images/training.png)
	![inference](images/inference.png)
1. Create an AWS Account
1. Apply AWS Credits
	> In your AWS account, your AWS Account ID can be found under 'My Account', which is itself found in the dropdown under the name of your account, between the bell and the 'Global' dropdown.
1. Check for GPU Access
1. [Setting up a Notebook Instance](https://www.youtube.com/watch?v=TRUCNy5Eqjc)
	> S3 stands for Simple Storage Service. It is Amazon's data storage service.
	> Also, using ml.t2.medium should be all that is necessary for the notebooks that you will encounter in this module. In addition, an ml.t2.medium instance is covered under the free tier.
1. [Getting the Notebooks](https://www.youtube.com/watch?v=jqL74whe9yo)
	```
	cd SageMaker
	git clone https://github.com/udacity/sagemaker-deployment.git
	exit
	```
1. Is Everything Set Up?
1. [Boston Housing Example: Getting the data Ready](https://www.youtube.com/watch?v=78y5cTR-JxM)
	> Session - A session is a special object that allows you to do things like manage data in S3 and create and train any machine learning models; you can read more about the functions that can be called on a session, at this documentation. The upload_data function should be close to the top of the list! You'll also see functions like train, tune, and create_model all of which we'll go over in more detail, later.
	> Role - Sometimes called the execution role, this is the IAM role that you created when you created your notebook instance. The role basically defines how data that your notebook uses/creates will be stored. You can even try printing out the role with print(role) to see the details of this creation.
	> In addition, we will be using a random tree model. In particular, we will be using the [XGBoost algorithm](https://xgboost.readthedocs.io/en/latest/)
	> Batch Transform is the method we will be using to test our model once we have trained it. 
	> High Level describes the API we will be using to get SageMaker to perform various machine learning tasks. In particular, it refers to the Python SDK whose documentation can be found here: https://sagemaker.readthedocs.io/en/latest/. This high level approach simplifies a lot of the details when working with SageMaker and can be very useful.