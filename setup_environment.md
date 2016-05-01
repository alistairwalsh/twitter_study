# Setup instructions

Once you have installed the Anaconda package manager, we can create an environment or 'env'.

This keeps different versions of libraries and Python versions seperate.

This part can be done from the command line

The environment can be created with	
	
	conda create -n positive anaconda nltk tweepy -c https://conda.binstar.org/lebpride
	
and activated with

	source activate positive
	
Or you can use the Anaconda GUI to create the env and activate it.

###Creating and using .yaml files to share your environment with others

After I installed all the libraries I created a .yaml file from it using

	conda env export > positive.yml

The .yaml file can be shared and used to setup the environment like this

	conda env create -f positive.yml