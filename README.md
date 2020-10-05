# challenge_docker
to properly use Docker and the important concepts of it: 
* Images
* Containers
* Volumes

## Objectives:

* Create your own Dockerfile.
* Build a Docker image.
* Run a Docker container.
* Add a Docker volume to your container.
* Manage your images
* Manage your containers



The Mission
You work for a company that creates ML models and ships them to their customer using APIs. Your team leader want to ship the next project using docker. He asks you to understand the basics of Docker in order to be effective for the next project.
WARNING: For this challenge you have to put your dockerfile in an isolated folder named docker. It's not a best practice at all (do not do that later). The goal is to learn how you can build your image from a different folder than the folder where you have you code.
You will reproduce the architecture of your collegues. Here it is:
/app
    |-docker
    |   |-Dockerfile -> your Dockerfile
    |-pipeline
    |   |
    |   |-model
    |   |    |-model.py -> print a number between 1 and 400
    |   |-preprocessing
    |   |    |-preprocessing.py -> print a numpy array
    |   |-utils
    |   |    |-utils.py -> print "in progress..."
    
### Steps
[] Create a github repository.
[] Create the above directory structure in it.
[] Create a Dockerfile that copy those files in an /app folder and run the model.py file.
[] Build your image
[] Run a container and verify that it prints the ouput of your model.py file.
[] Connect to your container with SSH and run all the python files model.py, preprocessing.py, utils.py
[] Stop you container and delete it (check that there are no more containers running with docker container ls -a)
[] Run a new container using a volume to do changes without stopping the container and saving your changes. Connect to SSH so it stays running.
[] Add two lines of code in each files locally (be creative!)
[] Re-run all your python files to verify that the changes are effective in your container.
[] Delete all your containers and images.
[] Push your repo with your Dockerfile.


### Must-have features
A nicely commented Dockerfile
The same directory structure as above
There are no more images or containers on your system
    
    
