# aws-virtual-isolation-mechanisms
Apply the concepts and skills related to AWS’ virtual isolation mechanisms to establish a private computing environment
1. In account, create a VPC (named VPC1) in a region named Region1 (e.g., Ohio). In the VPC, create and attach an Internet Gateway. Then, create a public subnet (named Subnet1) and a private subnet (named Subnet2); note that, the route tables of these subnets should be
configured appropriately.
2. In another region named Region2 (e.g., Oregon), create another VPC (named VPC2) and a private subnet (named Subnet3) within the VPC.
3. Create a peering between VPC1 and VPC2; route tables should be appropriately reconfigured to allow ec2 instances deployed to VPC1 and VPC2 to be able to communicate with each other using private IP addresses only.
4. On instance to create own AWS image
5. Deploy a private ec2 instance (named Server1) to Subnet2; deploy a private ec2 instance (named Server2) to Subnet3. Both Server1 and Server2 use the AWS image created in step 4.
6. Run EchoServer on Server1 and Server2. Run EchoClient on Client and check if it is able to communicate with the EchoServer on Server1 and Server2.
7. Create a S3 bucket with the name of 559Assignment4 and upload some files to it. Create an AWS user with program access. Log onto Server1 with Client as step stone, and configure Server1 appropriately such that you are able to use the AWS CLI on Server1 to list the files in bucket.
