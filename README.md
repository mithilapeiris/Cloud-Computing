# 🌩️ Cloud Computing – Concepts & Notes  

This repository provides a **beginner-friendly guide to cloud computing**, explained step by step with simple examples and analogies. It’s structured like a learning journey, covering the basics (servers, cloud) up to advanced concepts (IAM, VPC, etc.).  

---

## 📖 Table of Contents
1. [Servers](#servers)  
2. [Cloud](#cloud)  
3. [BaaS & FaaS](#baas--faas)  
4. [Cloud Computing Concepts](#cloud-computing-concepts)  
5. [IAM & IDaaS](#iam--idaas)  
6. [IAM Policy Documents](#iam-policy-documents)  
7. [VPC, Shared VPC, Subnets, VPN](#vpc-shared-vpc-subnets-and-vpn)  
8. [Regions](#regions)  

---

## Servers  
A **server** is a computer or program that provides services/data to other computers (**clients**) over a network.  

- **Examples**: Web servers, file servers, mail servers  
- **Analogy**: Like a **restaurant kitchen** serving food to customers  
- **How it works**: Clients send requests → Server processes → Server responds  

---

## Cloud  
The **cloud** means using the internet to access computing resources instead of owning hardware.  

- **Analogy**: Like electricity — you don’t build a power plant, you just pay for what you use.  
- **Models**:  
  - **IaaS** → Infrastructure as a Service  
  - **PaaS** → Platform as a Service  
  - **SaaS** → Software as a Service  
  - **BaaS** → Backend as a Service  
  - **FaaS** → Function as a Service  

---

## BaaS & FaaS  

### BaaS (Backend as a Service)  
- Ready-made backend features: authentication, database, file storage  
- **Examples**: Firebase, AWS Amplify  
- **Analogy**: Renting a **restaurant kitchen** so you focus only on cooking  

### FaaS (Function as a Service)  
- Run small pieces of code on demand without managing servers  
- **Examples**: AWS Lambda, Google Cloud Functions  
- **Analogy**: A **vending machine** — runs only when requested  

---

## Cloud Computing Concepts  
- **On-Demand Service** → Access anytime  
- **Broad Network Access** → Available anywhere  
- **Resource Pooling** → Shared infrastructure  
- **Scalability** → Grow/shrink as needed  
- **Pay-as-you-go** → Only pay for what you use  

**Deployment Models**: Public, Private, Hybrid, Community  
**Service Models**: IaaS, PaaS, SaaS, BaaS, FaaS  

---

## IAM & IDaaS  

### IAM (Identity & Access Management)  
- Controls **who can access what**  
- Features: Authentication, Authorization, Roles, Audit logs  
- **Analogy**: A **security guard + access card system**  

### IDaaS (Identity as a Service)  
- Cloud-based IAM  
- Features: SSO, MFA, federated login  
- **Examples**: Okta, Auth0, Azure AD  
- **Analogy**: Outsourcing building security to a professional company  

---

## IAM Policy Documents  
- JSON-based documents that define permissions  
- Structure: **Version, Statement (Effect, Action, Resource, Condition)**  

**Example – S3 Read Access**  

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-bucket/*"
    }
  ]
}