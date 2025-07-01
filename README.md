# aws-vpc
created vpc and vpc peering
# AWS VPC with Two EC2 Instances (No Bastion, Public Setup)

## 🔧 Project Overview

This project sets up:
- A custom VPC
- Two EC2 instances with public IPs
- An Internet Gateway
- Routing tables for internet access
- VPC Peering between two instances (in different subnets or VPCs)

## 🌐 EC2 Details

| Instance | IP (Public)    | Role            |
|----------|----------------|-----------------|
| EC2-1    | 18.141.175.118    | Web Server      |
| EC2-2    | 13.212.10.232  | Peer/Monitor    |

## 🧪 How to Access

1. SSH into either instance:
   ```bash
   ssh -i my-key.pem ubuntu@<instance-public-ip>
   2. run python server
python3 -m http.server 8000 --bind 0.0.0.0

Visit in browser:

http://<public-ip>:8000
