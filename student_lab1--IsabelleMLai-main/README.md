[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=16202608&assignment_repo_type=AssignmentRepo)
# EEC174 AY Lab 1: Intro to Software Tools

**Student Name:** Isabelle Lai

Please complete Assignment1.ipynb and the questions below. 
____

## 1. SSH

**(a) What is the purpose of binding ports between your laptop, server and docker container?** 
Binding the ports tells you which ports your container will use. Docker containers are used to separate different processes of your application, so ports are important to access the individual processes.  

____

## 2. Git

**(a) What is a git repository? Explain specifically why you would want to track your code with a repository.**

A git repository is a container in a project that contains a history of all the changes made to your project. It is important to track your code so you can save every version of your code. This is useful if your computer crashes and recent changes to your code are not saved locally, as this allows you to recover previously saved versions of your code. It is also useful for debugging if you wish to make changes to your code that may not be successful, as you can review previous successful versions of your code and see which specific version of your code resulted in an issue.  
____

**(b) Explain what a branch is in git. Why do we use branches when working in a team on one project?**

In git, a branch is a pointer to a specific part of your code and its changes. Branches are useful because they isolate specific parts of your code that you may want to focus on while developing your code. When working in a team, different people can work on different parts of the project without interfering with the other parts of the project that others may be working on. 
____

**(c) What is the master/main branch? What is its purpose in terms of deployment in a software project.**

The master/main branch is line of code that is meant to be the most stable out of all the versions of your code. It is the main line of development. In terms of deployment, the main branch should hold all of the finalized code that users should be able to successfully use. This is the branch that is most likely going to be deployed as it should not have bugs. 
____

**(d) Explain what a pull request is and why its important. Briefly explain the entire software development cycle using git**

A pull request is a request to add finalized changes to the main version of code. This could be used when you are working on an individual branch and have successfully made changes that you would like to apply to the main branch. This is important as it allows you to more seamlessly apply changes made on your branch to the main code. For software development, you would start with a main branch and an initial version of your code. You would create a new branch for software development, where smaller offshoot branches would be made for smaller features. Pull requests would be made to merge your branches together and to the main branch after you have successfully coded each feature and aspect of your newly developed version of code.Tthe main branch would then be updated to be the newest version of working code that could be released for users. 
____

## Docker

**(a) In your own words, explain why Docker is so useful for programmers. (A good answer will discuss all the potential ways that Docker saves programmer time).**

Docker is used to allow programmers to package and run an application in isolated containers. Docker is useful in allowing programmers to keep parts of their code isolated so that it is easy to see where bugs may have been developed in the program. Containers also contain everything needed to run the application, so it makes it easy to work on the application despite differences on host machines that the programmer may be using. Containers can run simultaneously on a host, so this means continuous development is supported. 
____

**(b) Explain the difference between a Docker container and a Docker image.**

Docker images are read only files and they are a template that gets loaded onto the container to run it. Docker images are also used to share code and are reuseable, while containers are created and destroyed when making an application. Docker containers are meant to change and they are where the software that you code runs. 

____

**(c) Explain how Docker can be used to solve a dependency clash between a Computer Vision program and a control program that are both being developed on the same machine.**

Docker allows you to isolate the different parts of an application. Using separate containers for the two programs would let you use different dependencies for each container. Docker images would allow youto define the dependencies for a given container.
____

**(d) Can Docker be used to run a Linux library on Windows? Explain.**

Yes, Docker's containers allows you to run a Linux library on Windows as containers isolate the application code they contain, and with the correct image, the containers will contain evreything needed to run the application code on various machines and environments. 
____

**(e) Can Docker be used to run and develop the same project on different machines. Explain.**

Yes, Docker uses containers to package everything needed to run code contained in the container. Dependencies are included in the container, and multi-platform images can be created to prepare the container to be run on different types of hardware by including multiple variants of the application that are compatible with different machines.

____

**(f) In 1 to 3 sentences, explain how you can build a new Image from scratch**

Docker has a command 'FROM' that specifies the base image you would like to build your container on, and it is the image that other layeers of the image will be built on. Then the command 'WORKDIR' should be used to set the working directory, where your application code will be inside the container and where commands will run from. Then the command 'RUN' should be used to install dependencies, 'COPY' should be used to copy the application files into the Docker container, 'ENV' should be used to set the environment variable, and 'CMD' should be used to define the default command. 
____

## Python

**(a) Explain the advantages between an interpreted and compiled language. Specifically, in what situations would it be more advantageous to use Python over C++?**

A compiled language allows you to work more closely to your processor and is specific to your machine. It also runs faster and has better performance than an interpreted language, and errors will prevnt the code from compiling. An interpreted language is more user friendly in terms of learning to code, and can be used across different machines more easily. It would be more advantageous to use Python over C++ when you wish to run your code on different computers. Python would also be better when you wish to handle large data, or when you wish to rapidly code prototypes. 
____

**(b) Explain what Lists, Dictionaries, and Tuples in Python are. Then, please give an example scenario where you would use each of them**

Lists are a data type that stores multiple values of a specified type under a single variable name. Lists would be used when you want to store multiple data values of the same type that you wish to access under the same general name. Lists have indexing and search functions that allow you to order values, as well as the ability to add and remove data values.
Dictionaries are a data type that stores a list of key-value pairs. Dictionaries would be used when you would like to store a collection of data values where each data point has multiple elements or aspects associated with it. Dictionaries are typically not used for creating ordered lists of data points. 
Tuples are a data type that stores multiple types of data points. Tuples cannot be changed after they are defined, and they are best used in instances where you would like to store multiple types of information about a variable. Tuples can act like a list of constructor elements for a given variable.
____


