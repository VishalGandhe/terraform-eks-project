
# 🚀 terraform-eks-project

This project uses **Terraform** to provision a **highly available Amazon EKS (Elastic Kubernetes Service) cluster** with a custom **VPC network topology** across multiple availability zones in AWS. It includes modular definitions for VPC, subnets, NAT gateway, and EKS node groups.

---

## 📦 Features

- 📍 Custom VPC with public, private, and intra subnets
- 🛡️ NAT gateway and internet gateway setup
- ☸️ Amazon EKS cluster with managed node groups
- 🧩 Modular code for easy environment replication (`dev`, `prod`, etc.)
- 🌍 Easily switch AWS regions and availability zones
- 📜 Clean separation of variables and configurations

---

## 🗂️ Project Structure
terraform-eks/
├── 📁 .terraform/              → Terraform internal data (auto-generated)
├── 📄 .terraform.lock.hcl      → Dependency lock file for Terraform providers
├── 📄 terraform.tfstate        → Current state of infrastructure
├── 📄 terraform.tfstate.backup → Backup of last known state
├── 🧩 locals.tf                → Local variables (region, env, subnets, etc.)
├── 🌍 provider.tf              → AWS provider configuration
├── 🛠️ terraform.tf             → Main Terraform configuration file
├── 🌐 vpc.tf                   → VPC, subnet, NAT gateway, and route tables
└── ☸️ eks.tf                   → Amazon EKS cluster and managed node groups

