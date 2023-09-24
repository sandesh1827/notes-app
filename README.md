# notes-app
A Django Notes App deployed with Nginx as a reverse proxy. Manage and organize your notes securely with this web application.

![Screenshot 2023-09-24 104141](https://github.com/sandesh1827/notes-app/assets/132772443/6085831c-c93d-4da3-b1e7-3a3a80828b09.png)

Introduction 

This project involves deploying a Django Notes App using Nginx as a reverse proxy on an AWS EC2 instance. The application allows users to manage and organize their notes and features user authentication and a user-friendly web interface.

Prerequisites:

AWS Account: You should have an AWS account to create and manage an EC2 instance.

GitHub Account: You'll need a GitHub account to host your Django Notes App repository.

Basic Linux Knowledge: Familiarity with basic Linux commands is essential for working with an EC2 instance.

Python 3.x: Ensure Python 3.x is installed on your EC2 instance, as Django typically requires Python 3.

Django Knowledge: Familiarity with Django and setting up Django projects is necessary.

Docker Knowledge: Basic knowledge of Docker is required for containerizing your Django application.

Nginx Installation: You should know how to install and configure Nginx on a Linux server.

Security Groups and Firewall Rules: Understanding how to configure security groups and firewall rules on AWS to allow traffic on necessary ports (e.g., 8000) is 

important for security.

Project Steps

1. Clone the Repository
Clone the Django Notes App repository from GitHub.

! [Screenshot 2023-09-24 104442](https://github.com/sandesh1827/notes-app/assets/132772443/97815fad-f2a4-4ce4-a96e-9b0d8dc1239a.png)

2. Install Docker
 
Install Docker to containerize the Django application.

![Screenshot 2023-09-24 104917](https://github.com/sandesh1827/notes-app/assets/132772443/d44c3c8c-f924-4ebc-b747-edfbbfe71a60)

3. Build and Run Docker Container
   
Build the Docker image and run the container in daemon mode on port 8000.

![Screenshot 2023-09-24 105106](https://github.com/sandesh1827/notes-app/assets/132772443/7b95ee17-2750-4c28-8721-f073bb25053f)

![Screenshot 2023-09-24 105608](https://github.com/sandesh1827/notes-app/assets/132772443/f186f933-53bd-49e7-aaae-f735cd68077a)

![Screenshot 2023-09-24 105728](https://github.com/sandesh1827/notes-app/assets/132772443/9dbacf79-24ae-464b-a645-8c36f22c165f)

4. Nginx Reverse Proxy Configuration
   
Edit the Nginx configuration to set up a reverse proxy.

![Screenshot 2023-09-24 105922](https://github.com/sandesh1827/notes-app/assets/132772443/bacec776-b1f2-42e9-b6b8-b0b2411d4a56)

5. Add the reverse proxy configuration:

![Screenshot 2023-09-24 110552](https://github.com/sandesh1827/notes-app/assets/132772443/922b12c9-7286-4dab-a652-b77791e300c8)

6. Serve Static Files
 
Copy static files to the Nginx web root.

![Screenshot 2023-09-24 111557](https://github.com/sandesh1827/notes-app/assets/132772443/3854ce8d-538d-4dbf-bfe9-f8936f711dd1)

7. Test Your Deployment
   
Access your application in a web browser using your instance's public IP address.

![Screenshot 2023-09-24 111730](https://github.com/sandesh1827/notes-app/assets/132772443/2ebc1396-6e36-41d2-808a-4774cebeb2b0)

   Conclusion
   
You have successfully deployed your Django Notes App using Nginx as a reverse proxy on an AWS EC2 instance. Ensure that you have configured security groups and
firewall rules properly to allow traffic on the necessary ports for your application.
