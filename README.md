# Node.js Docker Sample

This repository contains a sample Node.js application built for learning containerization using Docker.

## Prerequisites

Before you begin, ensure that you have the following prerequisites installed on your local machine:

- Node.js (version 18)
- Docker

## Getting Started

To get started with this project, follow the steps below:

1. Clone this repository to your local machine:

   ```shell
   git clone https://github.com/suveshmoza/nodejs-docker-sample.git
   ```

2. Navigate to the project's directory:

   ```shell
   cd nodejs-docker-sample
   ```

3. Install the required dependencies:

   ```shell
   npm install
   ```

4. Start the Node.js application:

   ```shell
   npm start
   ```

   The application will be accessible at [http://localhost:8080](http://localhost:8080).

## Dockerizing the Application

This project includes a Dockerfile that allows you to containerize the Node.js application. To build and run the Docker container, follow these steps:

1. Build the Docker image:

   ```shell
   docker build -t nodejs-docker-sample .
   ```

2. Run the Docker container:

   ```shell
   docker run -p 3000:8080 nodejs-docker-sample
   ```

   The application will be accessible at [http://localhost:8080](http://localhost:8080) within the Docker container and accessible at [http://localhost:3000](http://localhost:3000) outside the Docker container.
