# Task 3 - Virtual Private Cloud (VPC) Configuration

## Objective
To create a secure VPC with public and private subnets and configure internet access control using route tables and gateways.

## Configuration Summary
- **VPC Name:** intern-vpc  
- **Region:** ap-south-1 (Mumbai)  
- **VPC CIDR:** 10.0.0.0/16  
- **Subnets:**
  - Public Subnet → 10.0.1.0/24 → Internet access via IGW  
  - Private Subnet → 10.0.2.0/24 → Isolated (no internet route)
- **Internet Gateway:** intern-igw (attached)
- **Route Tables:**
  - Public RT → 0.0.0.0/0 → IGW
  - Private RT → local only

## Outcome
- Public subnet has internet connectivity.
- Private subnet remains isolated.
- Demonstrates segmentation and secure cloud networking.
