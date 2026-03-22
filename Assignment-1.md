# Problem Statement:
Working for an organization, you are required to provide them a safe and secure environment for the deployment of their resources.
They might require different types of connectivity. Implement the following to fulfill the requirements of the company.

# Tasks To Be Performed:
1. Create a VPC with 120.0.0.0/16 CIDR block.
2. Create 1 public subnet 2 private subnets and make sure you connect a NAT gateway for internet connectivity to a private subnet

   
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/55cd94e2-f390-4c60-bf51-55a0c3d03569" />

-----------------------
# Step-by-Step: VPC + Public + Private + NAT Gateway
-----------------------------
## 🔹 Step 1: Create VPC
Go to AWS Console
Search → VPC
<img width="1577" height="558" alt="image" src="https://github.com/user-attachments/assets/aa8ebc26-c4f0-479d-bbf7-d53e7bd812ec" />
Click → Create VPC
<img width="1473" height="588" alt="image" src="https://github.com/user-attachments/assets/82a61ae2-23dc-48c0-b079-b966af3a0423" />
Select:
✅ VPC only
<img width="1487" height="436" alt="image" src="https://github.com/user-attachments/assets/7ae61848-03ba-465d-8b21-909fdf2a510c" />
Fill details:
Name: my-vpc
CIDR: 120.0.0.0/16
Click → Create VPC
<img width="967" height="705" alt="image" src="https://github.com/user-attachments/assets/c256382d-d5b5-49a5-91a3-8d5acacbe924" />
<img width="1913" height="545" alt="image" src="https://github.com/user-attachments/assets/7738721d-8d4d-4c41-9c88-af6900a15747" />

-----------------------------

