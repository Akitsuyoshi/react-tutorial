# React_tutorial

This is a React tutorial, ['tic tac toe game']().

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app)

The code is written with React.js and ES6.

### Prerequisite
1. installed Docker in your local machine
2. somewhat familiarity with Docker

First of all, you can pull this code.
```
$ git clone https://github.com/Akitsuyoshi/react-tutorial
```
Since it is implemented Dockerfile in here, I'd like to use container instead of local environment.

In order to run this tutorial, here is the way to follow..

```
// It builds the image, while adding specific name
$ docker build -t IMAGE_NAME .

// It confirms you that the image exist with the added name
$ docker images

// In background, docker run this image with binding local port 3000 to container's 3000
$ docker run -d -p 3000:3000 IMAGE_NAME
```
If you visit http://localhost:3000/, you can see this application running.

At last, this is the way to close
```
// It shows the container ID
$ docker container ls

// To stop the process with ID
$ docker stop CONTAINER_ID
```

This application is used in my [blog](https://medium.com/@Akitsuyoshi/react-tutorial-70ebc48eacbc)
