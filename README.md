# 🌐 Terraform AWS VPC – Production-Ready Infrastructure

## 📌 Overview

This project provisions a **highly available and production-grade AWS VPC infrastructure** using Terraform.

It includes:

* Multi-AZ architecture
* Public, Private, and Database subnets
* Internet Gateway & NAT Gateway
* Route Tables & Associations
* VPC Peering setup

---

## 🏗 Architecture

![image](terraform-aws-vpc/assets/88663911/d3053c41-4a02-450d-9938-a575740a71e1)

---

## 🛠 Tech Stack

* AWS (VPC, Subnets, IGW, NAT, Route Tables)
* Terraform (Infrastructure as Code)
* HCL (HashiCorp Configuration Language)

---

## 📁 Project Structure

```bash id="hy28ni"
.
├── main.tf          # Core infrastructure resources  
├── variables.tf     # Input variables  
├── outputs.tf       # Output values  
├── data.tf          # Data sources  
├── locals.tf        # Local variables  
├── peering.tf       # VPC peering configuration  
├── .gitignore  
├── images/          # Architecture diagrams  
```

---

## 🚀 Infrastructure Components

### 🌐 Networking

* Custom VPC
* CIDR block configuration
* DNS support enabled

### 🌍 Subnets

* Public subnets (for internet-facing resources)
* Private subnets (for application layer)
* Database subnets (isolated layer)

### 🔌 Connectivity

* Internet Gateway (IGW)
* NAT Gateway (for private subnet outbound access)

### 🛣 Routing

* Public Route Table → IGW
* Private Route Table → NAT
* Database Route Table

### 🔗 VPC Peering

* Connectivity between custom VPC and default VPC

---

## ⚙️ How to Use

### Step 1: Initialize Terraform

```bash id="mib7og"
terraform init
```

### Step 2: Validate Configuration

```bash id="0xssub"
terraform validate
```

### Step 3: Plan Infrastructure

```bash id="s7r6je"
terraform plan
```

### Step 4: Apply Infrastructure

```bash id="7r4plg"
terraform apply
```

### Step 5: Destroy (Cleanup)

```bash id="r9r4i2"
terraform destroy
```

---

## 🔐 Best Practices Implemented

* Modular and reusable code structure
* Separation of variables and outputs
* Use of locals for dynamic values
* High availability across multiple AZs
* Secure network segmentation

---

## 💼 Real-World Use Case

This project demonstrates how to:

* Design scalable AWS networking architecture
* Deploy production-ready infrastructure using Terraform
* Implement secure and isolated environments
* Enable communication between VPCs

---

## 📊 Future Enhancements

* Convert into reusable Terraform module
* Add EKS cluster provisioning
* Integrate CI/CD pipeline (GitHub Actions)
* Add remote backend (S3 + DynamoDB)

---

## 👨‍💻 Author

Santhosh Gurujupalli
