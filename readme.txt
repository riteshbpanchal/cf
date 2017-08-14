•	Create VPC
o	Cidr 10.0.0.0/16
•	Create subnets
o	Public subnet – 10.0.1.0/24 in first AZ
o	Private subnet – 10.0.3.0/24 in second AZ
•	Create IGW and attach it to the VPC
•	Create public route table and associate public subnet to it
•	Create route to internet via IGW in the public route table
•	Create NAT gateway in the public subnet
o	Create EIP
•	Create private route table and associate private subnet to it
•	Create route to internet via NAT gateway in the private route table
•	Create EC2 instance in public subnet with security group
•	Create Launch config and ASG with min 1 web server in public subnet

