# Second-Semester Exam Landing Page Project

Website IP Address: http://54.89.250.148/ <br>
Student ID: ALT/SOE/024/0992

## Project Overview

The Landing Page Project demonstrates deploying a static web page on an Nginx web server hosted on an AWS EC2 instance. This includes deploying an HTML page containing my details (a short bio) as a student of AltSchool Africa for my second-semester exam. The project highlights the following key skills and configurations:

* Setting up a Linux server environment.
* Installing and configuring the Nginx web server.
* Deploying a custom HTML page.

The deployed landing page introduces the project creator and provides relevant project details.

## Setup Instructions

Follow the steps below to replicate setting up the Landing Page Project as a Cloud Engineering student.

### 1. Provision an AWS EC2 Instance as a server to deploy the static website

* Log in to your AWS account and launch an EC2 instance.
* Choose an Ubuntu 24.04 AMI for the server.
* Select an appropriate instance type (e.g., `t2.micro`).
* Configure the security group to allow the following traffic:
    * HTTP (Port 80) for web traffic.
    * HTTPS (Port 443) for secure web traffic.
    * SSH (Port 22) for remote server access.

### 2. Install the Apache Web Server

Run the following commands on the server to install and start Apache:

```
sudo apt update
sudo apt install apache2
```

### 3. Deploy the HTML Landing Page

Navigate to the default web root directory of Nginx:
```
cd /var/www/html/
```
Remove the Apache2's default HTML file:
```
sudo rm index.html
```
Launch the VI Editor in Linux to paste your HTML code.
```
sudo vi index.html
```
Exit the editor by pressing `esc` then `:wq` to close the editor.

### 4. Verification

Open a browser and navigate to the [landing page](http://54.89.250.148/) to confirm the secure connection.

## Usage
Click [HERE](http://54.89.250.148/) to access the landing page.
