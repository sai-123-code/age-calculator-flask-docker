# Age-calculator-flask-docker-ECS
This repository contains a simple Flask web application that calculates the age based on a user's date of birth, deployed using Docker and AWS ECS with Fargate. The goal of this project is to understand how Docker works, how to create Docker images, how to containerize a Python Flask application, and how to deploy it on AWS.

## Project Overview
The application is an age calculator that:
Takes a user's name and date of birth as input.
Calculates the age in years and months based on the current date (July 08, 2025, 03:42 PM IST).
Displays the result on the same page with a styled interface using CSS.

## Technologies Used
- **Python 3.13**: For the Flask backend.  
- **Flask**: A micro web framework for building the application.  
- **HTML/CSS**: For the frontend interface.  
- **Docker**: For containerizing the application.
- **AWS IAM**: For authenticating and managing access to AWS services.
- **AWS ECR**: For storing and managing Docker images.
- **AWS ECS with Fargate**: For deploying and running the containerized application.
- **AWS Security Groups**: For controlling network access to the ECS service.


## Build the Docker Image
docker build -t calculate_age .
## Run the Container
docker run -p 8080:5000 calculate_age
## For Pushing Docker image to AWS ECR
Refer to this offical AWS blog - https://docs.aws.amazon.com/AmazonECR/latest/userguide/docker-push-ecr-image.html

## Screenshots of Docker image created 
<img width="954" alt="Screenshot 2025-07-08 142403" src="https://github.com/user-attachments/assets/6180cf4e-b178-4b48-8b2e-b01907e955de" />

## Screenshots of Webpage running in docker container
<img width="956" alt="Screenshot 2025-07-08 142036" src="https://github.com/user-attachments/assets/c314083f-3ba1-48c2-a6d5-3aa52e1e57cc" />

## Screenshot of pushing Docker image to ECR using Amazon CLI
<img width="949" alt="Screenshot 2025-07-09 155849" src="https://github.com/user-attachments/assets/22ca1a2b-f7d0-4c93-a741-747a231106e9" />

##  Screenshot of creating ECS Cluster and related task definition with Fargate
<img width="942" alt="Screenshot 2025-07-09 175456" src="https://github.com/user-attachments/assets/39960c83-3fd3-4121-af17-5bf6b195000c" />

## Screenshot of final webapp deployed in same public ip address
<img width="959" alt="image" src="https://github.com/user-attachments/assets/f798abd6-8a04-45a1-9650-6ce8eef97a33" />




