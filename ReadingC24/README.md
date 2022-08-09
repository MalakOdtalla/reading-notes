## Django for APIs

Traditional Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

this [site](https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners) for full tutorial of how to create a REST API with Django REST framework.

## Docker
 Docker is a software platform that simplifies the process of building, running, managing and distributing applications. It does this by virtualizing the operating system of the computer on which it is installed and running.

 Docker Terminology:

 - Docker Image: is a template that contains the application, and all the dependencies required to run that application on Docker
 - Docker Container: is a logical entity. In more precise terms, it is a running instance of the Docker Image.
 - Docker Hub: is the official online repository where you could find all the Docker Images that are available for us to use.

 ### The Advantages and Disadvantages of using Docker
 Advantages:
 - Docker supports multiple applications with different application requirements and dependencies, to be hosted together on the same host, as long as they have the same operating system requirements.
 - Reduces costs. Docker is less demanding when it comes to the hardware required to run it.
 - Robustness. A container does not have an operating system installed on it. Thus, it consumes very little memory in comparison to a virtual machine (which would have a complete operating system installed and running on it).

 Disadvantages :
- Applications with different operating system requirements cannot be hosted together on the same Docker Host