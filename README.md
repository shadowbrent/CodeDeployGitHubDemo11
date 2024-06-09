Project Summary: AWS RDS Deployment with VPC Subnets and S3 Storage
Overview
This project involves deploying an AWS RDS database within a Virtual Private Cloud (VPC) configured with both public and private subnets, and storing database backups in Amazon S3. The goal was to ensure high availability, security, and durability of the database data.

Key Components

VPC Creation & Configuration
Subnets: Created public and private subnets.

Security Groups
RDS Security Group: Allowed inbound traffic on the database port.
EC2 Security Group: Allowed SSH access for management purposes.


RDS Deployment
Database Instance: Deployed an RDS instance in the private subnet for enhanced security.
Backup Configuration: Enabled automatic backups and configured them to be stored in Amazon S3.

EC2 Instance
Management Instance: Deployed an EC2 instance in the public subnet to manage and access the RDS instance securely.

S3 Integration
Backup Storage: Created an S3 bucket to store RDS backups.
Permissions: Configured IAM roles to grant RDS permission to write backups to the S3 bucket.

Testing and Verification
Connectivity: Verified access to the RDS database from the EC2 instance.
Backups: Confirmed that database backups were successfully stored in the S3 bucket.