# A dive into Amazon Virtual Private Cloud
   Before setting up infrastructures on your cloud space, it is of best practises to 
   setup a custom VPC for your project as it provides better security for you infrastructures
   and data.

## What is a Virtual Private Cloud (VPC)
   A Virtual Private Cloud (VPC) is a service offered by AWS and other cloud providers that allows 
   users to create a logically isolated section of the cloud. It lets users create their own network 
   setup with things like IP addresses, subnets, and security controls. Users can run their resources, 
   like servers and databases, in this private space, keeping them separate from other users. VPCs 
   helps you manage your cloud environment and connect it to your on-premises systems if needed.

   **Below are some components of a VPC**

   **Subnets**: A subnet, or subnetworks, is a smaller network within a larger network, designed 
   to partition and manage IP addresses more efficiently. In a Virtual Private Cloud (VPC), subnets 
   help organize resources by grouping them based on specific criteria, such as function or security level.
   There exist Private subnets (Which is a subnet with doesn't allow access from external sources except via the use
   of a Gateway) and Public Subnets (Which allows access from external sources).

   **Route Tables**: These define how traffic is directed within the VPC and between different subnets.
   They contain rules for routing traffic.

   **Internet Gateway**: A gateway that allows communication between resources in the VPC and the internet.
   It is essential for public subnets.

   **NAT Gateway/Instance**: Allows instances in a private subnet to access the internet while preventing
   inbound traffic from the internet. 

   **Below are some Advantages of using VPCs**
   

   **Isolation and Security**: VPCs provide a dedicated environment, isolating resources from other users
   and enhancing security through customizable security groups and network access control lists.

   **Customizable Network Configuration**: Users can define their own IP address ranges, subnets, and route 
   tables, tailoring the network to specific needs and applications.

   **Control Over Traffic**: VPCs allow for fine-grained control over inbound and outbound traffic, making
   it easier to enforce security measures and manage data flow.

   **Public and Private Subnets**: VPCs enable the creation of both public and private subnets, allowing
   sensitive resources to be isolated from direct internet access while still providing internet access to public resources. 
