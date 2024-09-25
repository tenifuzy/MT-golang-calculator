# MT-golang-calculator

A simple command-line calculator application built with Go and containerized using Docker.

## Description

This project implements a basic calculator that can perform addition, subtraction, multiplication, and division operations. It's written in Go and packaged in a Docker container for easy deployment and use.

## Docker Details

The project uses a multi-stage Docker build:
1. The first stage uses Ubuntu as the base image to build the Go application.
2. The second stage uses a `scratch` image to create a minimal final container with just the compiled binary.

## Project Structure

- `calculator.go`: Contains the Go code for the calculator application.
- `Dockerfile`: Defines the Docker image for the application.
- `README.md`: This file, containing project documentation.


## Prerequisites

- Docker
- Golang application

## Building the Application

To build the Docker image, run the following command in the project root directory:

docker build -t calculator .
This command builds a Docker image tagged as `calculator`.

![Screenshot (293)](https://github.com/user-attachments/assets/91e5b3a0-186e-4177-9445-962a1a180647)


## Running the Application

To run the calculator in a Docker container, use the following command:

docker run -it calculator
This command starts the calculator application in interactive mode, allowing you to input calculations.

![Screenshot (294)](https://github.com/user-attachments/assets/2fe023fb-9a4e-44d6-8f7f-420ae2b3a334)


## Viewing the image in Docker Desktop

![Screenshot (295)](https://github.com/user-attachments/assets/fac28f05-3025-4654-8b04-e63fc92d0877)

![Screenshot (296)](https://github.com/user-attachments/assets/59e0f3ed-c82b-473b-8072-e8f6a6bb1f8e)




