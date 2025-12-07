Designed and automated the provisioning of a custom AWS Virtual Private Cloud (VPC) using Terraform to support the MS Cleaning Service. The solution enforces network segmentation and security best practices, delivering a scalable, fault‑tolerant, and highly available architecture across three availability zones (eu‑west‑2a, eu‑west‑2b, eu‑west‑2c). Public and private subnets are provisioned with dedicated route tables, ensuring secure isolation of internal workloads while maintaining accessibility for internet‑facing applications through an Internet Gateway. DNS support enables seamless internal name resolution, while Terraform scripts orchestrate the entire deployment for consistency, compliance, and future scalability. This IaC‑driven model reduces manual configuration errors, optimizes resource allocation, and streamlines long‑term infrastructure management.

## Project Summary

This project automates the provisioning of a **custom AWS Virtual Private Cloud (VPC)** using Terraform, ensuring a scalable, secure, and highly available network architecture for the **MS Cleaning Service**. By eliminating manual intervention, this setup enables efficient resource management while maintaining flexibility for future expansions. The infrastructure is built around a **VPC with DNS support**, allowing seamless internal name resolution. Public and private subnets are provisioned across three availability zones (`eu-west-2a`, `eu-west-2b`, and `eu-west-2c`) to enhance fault tolerance and high availability. Each public subnet is configured to map public IP addresses upon instance launch, ensuring accessibility for internet-facing workloads. Connectivity is established through an **Internet Gateway (IGW)**, which allows resources within the public subnets to communicate externally. A dedicated **public route table** is created and associated with all public subnets, directing outbound traffic through the IGW. Similarly, private subnets are isolated with a **private route table**, ensuring internal communication while preventing direct exposure to the internet. Security considerations are integrated through **network segmentation**, where private subnets remain shielded while public-facing applications operate within designated subnets. This setup allows for better **resource isolation**, minimizing potential attack vectors while maintaining accessibility for necessary operations. Terraform scripts orchestrate the entire deployment, ensuring consistency and easy modification as infrastructure needs evolve. This **automated provisioning model** optimizes scalability, reduces manual configuration errors, and streamlines network resource allocation for long-term efficiency.

## The Implementation Steps are summarised below:

1️⃣ ### **Prerequisites**

Ensure you have the following installed:

  - **Terraform CLI** → [Download Terraform](https://developer.hashicorp.com/terraform/downloads)

  - **AWS CLI** → [Download AWS CLI](https://aws.amazon.com/cli/)

  - **Valid AWS Credentials** (`aws configure`)


## **2️⃣ Define Terraform Configuration Files**

## **3️⃣ Create a VPC**

## **4️⃣ Provision Subnets**

## **5️⃣ Create an Internet Gateway & Route Table**

## **6️⃣ Associate Subnets with Route Table**

## **7️⃣ Deploy Security Groups**

## **8️⃣ Initialize & Apply Terraform**

## **9️⃣ Verify Deployment**

## **🔹 Conclusion**

  ## **🔹 Why Automate VPC Creation?**

Overall, the **Automation of the provisioning of custom-built VPC with Terraform ensures consistency, scalability, and efficient and faster infrastructure deployment.**

