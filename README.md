# Network-Security-Project-with-AWS
Explore AWS networking &amp; security with a web app deployed on EC2 in a VPC. Public &amp; private services handle product data storage &amp; retrieval via RESTful APIs.

# Network & Security Project with AWS

Welcome to my Network & Security project repository! In this project, I've explored the concepts of Virtual Private Clouds (VPCs) and AWS RDS on Amazon Web Services. This project aims to showcase my understanding of these networking and security mechanisms.

## Overview
I've developed a containerized web services using Docker that runs on an EC2 instance within public subnet inside a VPC. The application has both public-facing and private services, each serving specific purposes. The application allows for the storage and retrieval of product data using RESTful endpoints. And deployed AWS RDS MySQL DB in private subnet and configured Security Group to allow EC2 in public subnet to interact with it. Configured Internet Gateway within VPC and public subnet routing table to allow internet access to EC2 in public subnet.

## Features
- Public-facing service accessible via a Public IP or Elastic IP.
- Private service within the VPC.
- RESTful API endpoints:
  - `/store-products`: Accepts JSON data and adds products to the database.
  - `/list-products`: Retrieves a list of products from the database.

![Alt text](https://github.com/pateljay15/Network-Security-Project-with-AWS/blob/main/A2/Architecture%20Diagarm.png)

## Usage
1. Clone this repository
2. Configure your AWS credentials to interact with AWS services.
3. Deploy the web application to an EC2 instance within a VPC.
4. Access the application via the assigned IP addresses.
5. Use the provided API endpoints to store and list products.

## Notes
- I've followed best practices and taken care to implement secure networking.
- Code snippets from external sources are properly cited and modified.
- I recommend checking AWS documentation for further assistance.

