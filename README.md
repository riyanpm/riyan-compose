# Riyan Docker Compose Project

## AWS Internship - Category 2

### Project Overview
This project demonstrates how to deploy and manage
multiple web servers using Docker and Docker Compose
on an AWS EC2 Ubuntu instance.

## Technologies Used
- Amazon EC2 (Ubuntu)
- Docker
- Docker Compose
- Nginx Web Server
- Apache HTTP Server
- Git and GitHub

## Project Structure

riyan-compose/
- compose.yaml
- nginx-site/index.html
- apache-site/index.html
- .gitignore
- README.md

## Docker Services

### 1. Nginx Website
- Image: nginx:stable
- Container: riyan-compose-nginx
- Port: 8083

### 2. Apache Website
- Image: httpd:2.4
- Container: riyan-compose-studio
- Port: 8084

## Run the Project

Clone the repository:

git clone https://github.com/riyanpm/riyan-compose.git

cd riyan-compose

Start containers:

sudo docker compose up -d

Check running containers:

sudo docker compose ps

## Test Websites

Nginx:
http://localhost:8083

Apache:
http://localhost:8084

For external access, replace localhost with the
EC2 public IP and allow the required ports
in the EC2 security group.

## Verification

Both web servers were tested successfully
and returned HTTP 200 OK.

## Git and GitHub

The project was version-controlled using Git
and pushed to a public GitHub repository.

## Conclusion

Successfully deployed two web servers using
Docker Compose on AWS EC2 and uploaded
the project source code to GitHub.
