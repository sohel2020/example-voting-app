Docker Voting App with CICD using Jenkins,Github,and DTR
===================

This app is used to help you construct a full CICD pipeline using Jenkins, Github, and DTR. This is based on the [example voting app](https://github.com/docker/example-voting-app) with multiple services. It is run with Docker Compose and uses Docker Networking to connect containers together. 

![](images/9_image_1.png)

Architecture
-----

* A Python webapp which lets you vote between two options
* A Redis queue which collects new votes
* A Java worker which consumes votes and stores them in…
* A Postgres database backed by a Docker volume
* A Node.js webapp which shows the results of the voting in real time

Running the App
-------

This app requires special instructions to be deployed as instructed in Lab #9 in [Docker Tutorials Repo](https://github.com/docker/dceu_tutorials/blob/master/9-cicd-with-docker.md).

The app will be running on port 5000 on your Docker host, and the results will be on port 5001.
