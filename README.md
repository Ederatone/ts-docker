A minimal TypeScript application demonstrating various Docker containerization strategies, including multi-stage builds and Alpine-based images.

## Overview
This project showcases:

- A simple Express.js server written in TypeScript

- Multiple Dockerfile configurations:

    - Dockerfile: Basic setup

    - Dockerfile.alpine: Lightweight Alpine-based image

    - Dockerfile.multistage: Multi-stage build for optimized image size

    - Dockerfile.optimized: Further optimized production image

- Docker Compose integration for streamlined development and deployment

## Getting Started
### Prerequisites
- Node.js (v14 or later)
- Docker
- Docker Compose
### Installation
1. Clone the repository:
```
git clone https://github.com/Ederatone/ts-docker.git
cd ts-docker
```
2. Install dependencies:
```
npm install
```
3. Build the TypeScript project:
```
npm run build
```
## Running the Application
### Using Docker
Build and run the Docker container:
```
docker build -f Dockerfile -t ts-docker-app .
docker run -p 3000:3000 ts-docker-app
```
Using Docker Compose
Start the application using Docker Compose:
```
docker-compose up --build
```
## Available Scripts
- **npm run build**: Compile TypeScript to JavaScript
- **npm run start**: Run the compiled JavaScript
- **npm run dev**: Start the application in development mode with hot-reloading
# Project Structure
```
ts-docker/
├── src/                 # TypeScript source files
├── dist/                # Compiled JavaScript files
├── Dockerfile           # Basic Docker configuration
├── Dockerfile.alpine    # Alpine-based Docker configuration
├── Dockerfile.multistage# Multi-stage build Docker configuration
├── Dockerfile.optimized # Optimized production Docker configuration
├── docker-compose.yml   # Docker Compose configuration
├── package.json         # Node.js project metadata and scripts
├── tsconfig.json        # TypeScript compiler configuration
└── README.md            # Project documentation
```