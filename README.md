# My Node.js App

This is a simple Node.js application that runs inside a Docker container.

## Getting Started

### Prerequisites

- Docker
- Docker Compose

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/my-node-app.git
    cd my-node-app
    ```

2. Build and run the Docker container:
    ```sh
    docker-compose up -d
    ```

3. Access the application:
    - Go to `http://localhost:3000` if running locally.
    - Go to `http://your-ec2-public-dns:3000` if running on AWS EC2.

### commands 

 To run without docker compose use

  $ docker build -t nodeproject-web .

  $ docker run -p 3000:3000 nodeproject-web

 To run with docker compose
   
   $ docker compose up

## General Docker Commands

- `docker images`  
  To list images

- `docker ps -a`  
  To list containers

- `docker stop <container id>`  
  To stop a running container

- `docker rm <container id>`  
  To delete containers

- `docker rmi <image name>`  
  To delete Docker images

- `docker system prune -a`  
  To delete all images and containers

## Running a Docker Container in the Background

- `docker run -d <image name>`  
  To run a Docker container in the background (detached mode)

## Tagging a Docker Image

- `docker tag <existing-image-id> <new-repository-name>:<tag>`  
  To tag an existing Docker image






### Files

- `app.js`: The main Node.js application file.
- `Dockerfile`: The Dockerfile used to build the Docker image.
- `docker-compose.yml`: The Docker Compose file to manage the services.

### Built With

- [Node.js](https://nodejs.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

C
