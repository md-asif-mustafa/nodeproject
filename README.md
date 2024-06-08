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

General docker commands
   docker images               / to list images
   docker ps -a                / to list containers
   docker stop <container id>  / to stop running container 
   docker rm <container id>    / to delete containers
   docker rmi <image name>     / to delete docker images




### Files

- `app.js`: The main Node.js application file.
- `Dockerfile`: The Dockerfile used to build the Docker image.
- `docker-compose.yml`: The Docker Compose file to manage the services.

### Built With

- [Node.js](https://nodejs.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

C
