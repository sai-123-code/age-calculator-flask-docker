# Age-calculator-flask-docker
This repository contains a simple Flask web application that calculates the age based on a user's date of birth, deployed using Docker. The goal of this project is to understand how Docker works, how to create Docker images, and how to containerize a Python Flask application.

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


## Build the Docker Image
docker build -t flask-age-calculator .
## Run the Container
docker run -p 8080:5000 flask-age-calculator

## Screenshots of Docker image created 
<img width="954" alt="Screenshot 2025-07-08 142403" src="https://github.com/user-attachments/assets/6180cf4e-b178-4b48-8b2e-b01907e955de" />

## Screenshots of Webpage running in docker container
<img width="956" alt="Screenshot 2025-07-08 142036" src="https://github.com/user-attachments/assets/c314083f-3ba1-48c2-a6d5-3aa52e1e57cc" />
