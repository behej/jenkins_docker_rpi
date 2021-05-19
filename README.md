# Jenkins
Docker image for Jenkins CI.
This image runs Jenkins but also development tools such as:
* gcc
* make
* git
* python

Do not forget to mount volume for permanent storage of date (plugins, jobs configuration, etc.)

## Usage
```
docker run --rm --name jenkins -p 8080:8080 -p 50000:50000 -v path/to/volume:/var/jenkins_home jeromebehe/jenkins-rpi:latest
```




## Versions
* 1.0 : Jenkins version 2.277.4
* 1.1 : Add Git, make and gcc
* 1.2 : Add python 3.8

