## Introduction
In this project, I successfully deployed a website on AWS, utilizing **Git for version control**, **Linux for development**, and **EC2 for hosting**. Below is a detailed breakdown of the steps I followed.
## 1. Git Repository Setup
- I installed Git on my system.
- I initialized my repository:
  ```bash
  git init
•	mkdir MarketPeak_Ecommerce
•	cd MarketPeak_Ecommerce
•	git init
•	I configured my Git settings: 
•	git config --global user.name "Oyebola Olowoyeye"
•	git config --global user.email "deboaster2003@gmail.com"
•	I added and committed my files: 
•	git add .
•	git commit -m "Initial commit"

2. Branching & Development
•	I created and switched to a development branch: 
•	git checkout -b development
•	I continued development on this branch to keep changes organized.
•	I regularly committed updates to maintain version control.
3. Linux Development Environment
•	I set up my development environment on Amazon Linux.
•	I installed necessary dependencies and tested my workflow.
4. AWS EC2 Setup
•	I launched an EC2 instance using Amazon Linux 2023 AMI.
•	I connected to my instance via SSH: 
•	ssh -i my-key.pem ec2-user@my-instance-ip
5. Web Server Installation & Configuration
•	I installed Apache: 
•	sudo yum update -y
•	sudo yum install httpd -y
•	I started and enabled the web server: 
•	sudo systemctl start httpd
•	sudo systemctl enable httpd
•	I configured the server to host my website.
6. Website Deployment
•	I transferred my website files: 
•	sudo rm -rf /var/www/html/*
•	sudo cp -r ~/MarketPeak_Ecommerce/* /var/www/html/
7. Website Accessibility
•	I modified AWS security groups to allow HTTP traffic.
•	I accessed my website via the public IP of the EC2 instance.
8. Merging & Repository Sharing
•	I merged my development branch into the main branch: 
•	git checkout main
•	git merge development
•	I pushed the repository to GitHub: 
•	git push origin main
•	I shared my repository as part of the capstone submission.
9. README.md Documentation
I created a detailed README.md file, outlining:
# My Capstone Project
## Project Overview
This project involved deploying a website using AWS EC2 and Git version control.
________________________________________

