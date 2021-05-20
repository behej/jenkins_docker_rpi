# Jenkins
Docker image for Jenkins CI.
This image runs Jenkins but also development tools such as:
* gcc
* make
* git
* python, pip and other packages

Do not forget to mount volume for permanent storage of date (plugins, jobs configuration, etc.)

## Usage
```
docker run --rm --name jenkins -p 8080:8080 -p 50000:50000 -v path/to/volume:/var/jenkins_home jeromebehe/jenkins-rpi:latest
```



## Changelog
* 1.3 : Add pip and nosetests
* 1.2 : Add python3.8
* 1.1 : Add Git, make and gcc
* 1.0 : Jenkins version 2.277.4


