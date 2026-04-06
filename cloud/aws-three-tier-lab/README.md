# AWS Three-Tier Lab (Ephemeral)

## Overview
This project demonstrates a low-cost, ephemeral three-tier architecture in AWS.  
The goal is to showcase VPC design, subnet segmentation, EC2 deployment, and secure communication between tiers.

The environment is designed to be created, tested, documented, and then destroyed to minimize cost.

---

## Architecture Goals
- Custom VPC design
- Separation of web, application, and database tiers
- Public and private subnet configuration
- Secure communication between tiers
- Minimal cost and short runtime

---

## High-Level Checklist
- Build a custom AWS VPC for a three-tier lab environment
- Separate the environment into web, application, and database tiers
- Use public and private subnet design to control exposure
- Configure route tables, internet access, and internal-only communication paths
- Deploy EC2 instances for the web and application layers
- Deploy a private database layer
- Apply security groups to restrict traffic between tiers
- Use IAM roles and secure administration practices
- Validate tier-to-tier connectivity and application functionality
- Capture architecture screenshots and deployment evidence
- Document security decisions, networking layout, and lessons learned
- Tear down the environment after testing to keep costs low
- Publish final documentation and results

---

## Planned Features
- Simple inventory/task web app
- Frontend (web tier)
- Backend API (application tier)
- Database (data tier)
- End-to-end communication validation

---

## Status
🚧 In Progress