# docker-java8-mvn-nodejs-npm
I was unable to find an image which could build both java and npm projects, so I created one myself.

This image is mainly to build projects which have java and nodejs in one umbrella.
It contains the latest version of java8, maven, nodejs, and npm.

Basically, I just combine the public docker build file of these three projects together:
* [https://github.com/docker-library/java/blob/6f340724d3bc1f9b4385975c5de6bfe15aac8c85/openjdk-8-jdk/Dockerfile](https://github.com/docker-library/java/blob/6f340724d3bc1f9b4385975c5de6bfe15aac8c85/openjdk-8-jdk/Dockerfile)
* [https://github.com/carlossg/docker-maven/blob/882a21728d702dad08279afe6b6bf9fa4b8bfe18/jdk-8/Dockerfile](https://github.com/carlossg/docker-maven/blob/882a21728d702dad08279afe6b6bf9fa4b8bfe18/jdk-8/Dockerfile)
* [https://github.com/nodejs/docker-node/blob/d798690bdae91174715ac083e31198674f044b68/0.12/wheezy/Dockerfile](https://github.com/nodejs/docker-node/blob/d798690bdae91174715ac083e31198674f044b68/0.12/wheezy/Dockerfile)

All credits should go to the ones who created those.
