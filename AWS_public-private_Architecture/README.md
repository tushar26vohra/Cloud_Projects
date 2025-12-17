# AWS High Availability Web Application

## Overview
This project demonstrates a highly available web application architecture built on AWS using public and private subnets.

## Architecture
- One VPC with two Availability Zones
- Public subnets hosting an Application Load Balancer
- Private subnets hosting EC2 instances
- Internet Gateway for public access
- NAT Gateway for outbound internet access from private subnets
- Security Groups for traffic control

## Traffic Flow
User → Application Load Balancer → EC2 instances → Response

## Security
- EC2 instances are placed in private subnets
- Only the ALB can access EC2 instances
- SSH access is restricted

## Issue Faced & Fix
Initially, the Application Load Balancer was created as internal, which caused the application to be inaccessible from the browser.  


## What I Learned
- Difference between internal and internet-facing ALB
- Importance of security groups
- How AWS services integrate in real architectures
