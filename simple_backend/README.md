# Simple Express.js App with Docker Setup

This repository contains a basic Express.js application that serves a simple message. It's set up to be run using Docker for easy deployment and development.

## Prerequisites

Before you begin, make sure you have the following installed:

- Node.js (14 or later)
- Docker

## Getting Started

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/<chiemezie1>/simple_Docker_application-/.git
   cd simple_Docker_application-/simple_backen
    ```

1. **Install Dependencies:**
    
    Install the application dependencies using npm:
    
    ```bash
    npm install
    ```
    
2. **Run Locally:**
    
    To run the application locally without Docker, use:
    
    ```bash
    
    nodemon --exec babel-node index.js
    
    ```
    
    Open your browser and navigate to **[http://localhost:4000](http://localhost:4000/)** to see the message.
    

## **Using Docker**

1. **Build the Docker Image:**
    
    Build the Docker image for the application using the provided Dockerfile:
    
    ```bash
    bashCopy code
    docker build -t simple-express-app .
    
    ```
    
2. **Run the Docker Container:**
    
    Run the application as a Docker container:
    
    ```bash
    bashCopy code
    docker run -p 4000:4000 -d simple-express-app
    
    ```
    
    Access the app by opening your browser and navigating to **[http://localhost:4000](http://localhost:4000/)**.
    

## **Contributing**

Feel free to contribute by opening issues or pull requests in this repository. This is a simple setup, so any improvements or suggestions are welcome!

## **License**

This project is licensed under the MIT License - see the **[LICENSE](https://chat.openai.com/LICENSE)** file for details.