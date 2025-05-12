# -nodejs-demo-app
This is a simple Node.js application that returns a "Hello from Node.js App!" message.It's containerized using Docker and deployed using GitHub Actions.
 
 ## Tech Stack 
  - Node.js
  - Docker
  - GitHub Actions(CI/CD)

## Features 
- Simple HTTP server 
- Dockerized for easy deployment
- Automatedd build and push using GitHub Actions

##  Running Locally

Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/nodejs-demo-app.git
cd nodejs-demo-app
npm install
npm start

## Running with Docker

Build and run the Docker container:

```bash
docker build -t yourusername/nodejs-demo-app .
docker run -d -p 3000:3000 yourusername/nodejs-demo-app

## CI/CD with GitHub Actions

When you push to the `main` branch, GitHub Actions will:

- Build the app
- Create a Docker image
- Push it to DockerHub

Ensure these secrets are set in GitHub:
- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`




  