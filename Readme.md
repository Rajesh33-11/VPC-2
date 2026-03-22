Problem Statement:
	You are a cloud architect tasked with designing a secure and efficient Virtual Private
	Cloud (VPC) for a rapidly growing e-commerce platform. The platform currently
	operates in a single region but plans to expand to multiple regions in the future to
	improve availability and reduce latency for global customers. Keeping in mind the
	complexity and security of the architecture.

Objective:
	Design multiple VPC architectures that ensure high availability, scalability, and
	security for the e-commerce platform. The design should support future expansion to
	multiple regions while maintaining optimal performance for customers.


Requirements:

1. VPC Design:
● Create 3 VPCs, Prod-Net (N. Virgina), Dev-Net (N. Virgina) and Test-Net
(Oregon) with CIDR block 10.10.0.0/16, 11.11.0.0/16 and 20.20.0.0/16
respectively.
● Divide the VPC Prod-Net into 2 public and 3 private subnets to separate the
web application, database servers, and other services.
● Divide Dev-Net and Test-Net in one of each public and private subnets.

2. Subnets and Routes:

● Create subnets in each Availability Zone (AZ) for high availability and fault
tolerance in each of the VPCs.
● Configure route tables of public subnets in each VPC to direct traffic between
subnets and to the internet gateway for outbound internet access.
● Create a separate route table to direct traffic to private subnets using ANT
gateways. Make sure one private subnet is not attached to the Internet or NAT
gateway in each VPC.

3. VPC Peering:
● Set up VPC peering connections between the Dev-Net VPC and Test-Net VPC
in different regions for inter-region communication.

4. Transit Gateways:
● Consider using Transit Gateway to simplify the management of Dev-Net and Prod-Net VPCs.

5. Endpoints:
● Configure VPC endpoints for S3 to allow private access to this service without
going over the internet.
