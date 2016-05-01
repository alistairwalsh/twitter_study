# Setup instructions

Once you have installed the Anaconda package manager, we can create an environment or 'env'.

This keeps different versions of libraries and Python versions seperate.

This part can be done from the command line

	conda create -n positive anaconda nltk twython -c https://conda.binstar.org/dimazest
	
Notice I've added a channel with the -c flag. This is so twython can be installed


###Creating and using .yaml files to share your environment with others

After I installed all the libraries I created a .yml file from it using

	conda env export > positive.yml

The .yaml file can be shared and used to setup the environment like this

	conda env create -f positive.yml
	
but the https://conda.binstar.org/dimazest channel is required for twython so do this before running the .yml file

	conda config --add channels https://conda.binstar.org/dimazest



	
