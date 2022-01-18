## Intro to the Dockerfile Components

[Full article available on SweetCode for free](https://sweetcode.io/intro-to-the-dockerfile-components/) 

A major problem faced by many programmers and developers is how to properly configure a local development environment; this is despite all the advancements we have in modern programming languages. To help reduce all these conflicts in work, a solution was made: Docker. Even though it is relatively new in the industry, it has quickly won the hearts of many developers working on production-level projects.

In this article, we will be discussing a very important file associated with Docker: a Dockerfile. We will be discussing what it is, commands associated with it, how to write one, and its significance to developers.

Let's get started:

## What is a Dockerfile?

![what is a Dockerfile](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zev1564t65inedf0a53y.png)

It will be fair to state that in this article we will be juggling between some common terms associated with the Dockerfile, that is Docker, Docker Images, and Containers. Let's understand what these terms mean:

__*Docker*__ is an open-source project designed to make it easier to develop, deploy, and run applications by the use of containers. It allows developers to package up an application with all the parts it needs into a container, then ship it out mutually as one package.

__*Docker Container*__ is a software package that will include all dependencies required such as libraries, config files, etc… to run an application and ship them as one package.

__*Docker Image*__ is a snapshot of what a project contains and it is represented by a Dockerfile. This file contains everything that is needed to run an application. They are either using a predefined Image or using a Dockerfile

That being said, we can describe a Dockerfile as a text document that contains a series of commands that are used to automatically create containers and assemble an image on the Docker platform.

As defined it is a text document, also it’s important to state that the Dockerfile has no extension, all you need is to save it as Dockerfile

It is within the Dockerfile that applications, frameworks, servers, base images are specified.

All commands initiated in the Docker file are executed from top to bottom with each step being cached. Execution of these instructions takes place on a base image.

On building the Dockerfile, the successive actions form a new image from the base parent image which is specified in the file as the first command.

## Dockerfile Syntax

The Dockerfile syntax consists of two mainline blocks, that is the comment block and the command block.

**Syntax**
```dockerfile
# Comment
COMMAND argument
```

An example in a file:
```Dckerfile
# Prints greeting message
RUN echo "Greetings Team SweetCode"
```
The Commands are not usually case sensitive, but in order to differentiate them from the arguments, they are usually written in UPPERCASE and arguments in lowercase as shown above.

When writing a Dockerfile, there are a dozen of commands which can be specified inside the file. Let’s go ahead and have a look at the most commonly used.

## Dockerfile Commands 
Besides this we have common practices that are considered must in a Dockerfile, In each file, the first command will always be FROM command.

That being said, let’s begin:

**FROM**
It is considered the most crucial amongst all other commands in the Dockerfile. A Dockerfile MUST begin with the FROM command.

It defines the base image which will be used in the build process.

*Syntax*
```
FROM <Image name>
or
FROM <image>:<tag>
or
FROM <image>@<digest>
```
The image name defines where the new image should inherit from.
*Example*
```
FROM Ubuntu
```

What basically this command does is, tell the Docker builder to use this base image as a starting point. It’s going to download the latest Ubuntu version from the docker hub.

To learn more about all the Images we have, check out the Docker Hub here https://hub.docker.com/.

## Continue Reading:

Check out the complete Article on [SweetCode](https://sweetcode.io/intro-to-the-dockerfile-components/).

*No registration is needed to access the article*

Connect With me at [Twitter](https://twitter.com/larymak1) | [Insta](https://www.instagram.com/nextgencoders/) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi)  | 