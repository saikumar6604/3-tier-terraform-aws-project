# 🚀 3-Tier Web Application Deployment using Terraform (AWS)

## 📌 Project Overview

This project demonstrates the deployment of a **3-tier architecture** on AWS using **Terraform (Infrastructure as Code)**.

The architecture is designed to be **scalable, highly available, and automated**, following real-world DevOps practices.

---

## 🏗️ Architecture Overview

The application is divided into three layers:

### 🔹 1. Presentation Layer

* Implemented using **Application Load Balancer (ALB)**
* Distributes incoming traffic across multiple EC2 instances
* Improves availability and fault tolerance

### 🔹 2. Application Layer

* Implemented using **Auto Scaling Group (ASG)** with EC2 instances
* Uses a **Launch Template** to define instance configuration
* Automatically scales based on demand

### 🔹 3. Data Layer

* Implemented using **Amazon RDS (MySQL)**
* Stores application data securely
* Provides managed database service

---

## 🌐 Infrastructure Components

* **VPC (Virtual Private Cloud)**

  * Custom CIDR block
  * Isolated network environment

* **Subnets**

  * Public Subnets for ALB and EC2
  * Multi-AZ deployment for high availability

* **Internet Gateway**

  * Enables internet access

* **Route Tables**

  * Manages routing between subnets and internet

* **Security Groups**

  * Controls inbound and outbound traffic

---

## ⚙️ Key Features

✅ Infrastructure as Code using Terraform
✅ Modular and scalable architecture
✅ Auto Scaling for high availability
✅ Load balancing using ALB
✅ Automated EC2 provisioning using user data scripts
✅ Secure networking with VPC and Security Groups

---

## 🛠️ Tech Stack

* **Cloud Provider:** AWS
* **IaC Tool:** Terraform
* **Compute:** EC2 (Auto Scaling Group)
* **Load Balancer:** Application Load Balancer (ALB)
* **Database:** Amazon RDS (MySQL)
* **OS:** Linux
* **Scripting:** Bash

---

## 📂 Project Structure

```bash
3-tier-terraform-aws-project/
│
├── main.tf
├── provider.tf
├── variables.tf
├── outputs.tf
├── README.md
├── .gitignore
│
└── scripts/
    └── user_data.sh
```

---

## 🚀 How to Run the Project

### 🔹 Prerequisites

* AWS Account
* Terraform installed
* AWS CLI configured

### 🔹 Steps

```bash
terraform init
terraform plan
terraform apply
```

👉 Type `yes` to confirm deployment

---

## 📊 Output

After successful deployment:

* ALB DNS will be generated
* Open in browser to access application

---

## 🔐 Security Considerations

* Security groups allow only required ports (HTTP, SSH)
* Infrastructure isolated using VPC
* Sensitive values should be stored securely (future improvement)

---

## 📈 Future Enhancements

* Add **S3 backend for Terraform state**
* Implement **DynamoDB state locking**
* Deploy EC2 in **private subnets**
* Add **CI/CD pipeline using GitHub Actions**
* Use **Terraform modules for better reusability**

---

## 📌 Key Learnings

* Hands-on experience with AWS infrastructure
* Understanding of 3-tier architecture design
* Terraform resource creation and automation
* Working with ALB, ASG, and RDS
* Real-world DevOps project implementation

---

## 👨‍💻 Author

**Kamatam Prasanna Sai Kumar**
DevOps Enthusiast | AWS | Terraform | Kubernetes

---

## ⭐ Conclusion

This project showcases the practical implementation of cloud infrastructure using Terraform and demonstrates knowledge of scalable and resilient system design.

---
