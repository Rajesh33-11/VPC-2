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
- Go to AWS Console
- Search → VPC
<img width="1577" height="558" alt="image" src="https://github.com/user-attachments/assets/aa8ebc26-c4f0-479d-bbf7-d53e7bd812ec" />
- Click → Create VPC
<img width="1473" height="588" alt="image" src="https://github.com/user-attachments/assets/82a61ae2-23dc-48c0-b079-b966af3a0423" />
- Select:
✅ VPC only
<img width="1487" height="436" alt="image" src="https://github.com/user-attachments/assets/7ae61848-03ba-465d-8b21-909fdf2a510c" />

- Fill details: **Name: my-vpc  →  CIDR: 120.0.0.0/16  →  Click → Create VPC**
<img width="967" height="705" alt="image" src="https://github.com/user-attachments/assets/c256382d-d5b5-49a5-91a3-8d5acacbe924" />
<img width="1913" height="545" alt="image" src="https://github.com/user-attachments/assets/7738721d-8d4d-4c41-9c88-af6900a15747" />

-----------------------------
## 🔹 Step 2: Create Public Subnet
- Left side → Subnets
<img width="1042" height="596" alt="image" src="https://github.com/user-attachments/assets/489fc30a-24bb-4d92-b0a3-a08952ea63f9" />
- Click → Create subnet
<img width="1643" height="337" alt="image" src="https://github.com/user-attachments/assets/5fc65a7d-c514-43c7-9368-a61ffb2aa27d" />
- Select your VPC
- <img width="1533" height="422" alt="image" src="https://github.com/user-attachments/assets/1e5ed63e-94ec-46ae-9b74-35729fe5d3d0" 
     
- Enter: **Name: public-subnet  →  AZ: ap-south-1a  →   CIDR: 120.0.1.0/24 →  Click → Create subnet**
<img width="1595" height="772" alt="image" src="https://github.com/user-attachments/assets/60085e55-4835-4161-bf66-af655c0af8ac" />
<img width="1588" height="413" alt="image" src="https://github.com/user-attachments/assets/3ffd22fd-2b7e-43f0-a46d-ed2a1343fe2d" />

-----------------------------
## 🔹 Step 3: Create Private Subnets (2)
### Private Subnet 1 
**Name: private-subnet-1  →  AZ: ap-south-1a  →  CIDR: 120.0.2.0/24**
<img width="1701" height="758" alt="image" src="https://github.com/user-attachments/assets/852a1911-e6d7-446f-9907-08b2220a6ed3" />
👉 Click → Create subnet
<img width="1680" height="322" alt="image" src="https://github.com/user-attachments/assets/36720678-9dd6-4d2b-abd5-0d445bc18016" />

##### Private Subnet 2
**Name: private-subnet-2  →  AZ: ap-south-1b  →  CIDR: 120.0.3.0/24**
<img width="1602" height="757" alt="image" src="https://github.com/user-attachments/assets/3aa87bb0-5a25-46b4-81cc-be0384c2551e" />
👉 Click → Create subnet
<img width="1909" height="575" alt="image" src="https://github.com/user-attachments/assets/0cb256df-574a-4757-be56-41b6d31da9df" />

-----------------------------
## 🔹 Step 3: Create Private Subnets (2)
