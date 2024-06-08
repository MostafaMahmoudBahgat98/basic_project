# Simple CI Pipeline with Docker, Jenkins, and Git

This project demonstrates setting up a Continuous Integration (CI) pipeline for a simple web application(Task Manager) using Docker, Jenkins, and Git.

## Requirements

- Docker
- Jenkins
- Git

## Steps

### 1. Create a Simple Web Application

We'll be using Flask, a simple web framework in Python, to create a basic web application.

### 2. Writing Dockerfile

Define a Dockerfile to create an image of the application. Additionally, create a `requirements.txt` file listing all the Python dependencies required by the application.

### 3. Create a Jenkinsfile

Create a Jenkinsfile to define the Continuous Integration pipeline. This file will contain the steps for building, testing, and deploying the application.

### 4. Jenkins Setup

Ensure Jenkins is installed and running. Set up a new project in Jenkins, configure it to use the Jenkinsfile created in step 3, and define the build and run steps.

## Usage

1. Clone this repository:

   ```bash
   git clone <repository_url>
