## Steps Followed

1. Created a VPC with public and private subnets
2. Attached an Internet Gateway to the VPC
3. Created a NAT Gateway for private subnet internet access
4. Launched EC2 instances in private subnets
5. Installed a web server using Python HTTP server on port 8000
6. Created an Application Load Balancer in public subnets
7. Configured target groups and health checks
8. Fixed access issue by changing ALB to internet-facing
