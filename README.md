# Order Orchestrator 🎯

![AWS](https://img.shields.io/badge/AWS-Learning-yellow?logo=amazonaws) ![Git Submodules](https://img.shields.io/badge/Git-Submodules-orange?logo=git) ![Practice](https://img.shields.io/badge/Practice-Project-blue) ![Deployment](https://img.shields.io/badge/Deployment-Automation-green)

This repository orchestrates the **Ordering System Demo**, coordinating the Java-based `order-service` and Java-based `order-infra` (AWS CDK) for deployment. It’s a practice project to solidify my **AWS learning**, demonstrating how to tie application and infrastructure together.

## 🚀 Project Purpose
This project showcases my AWS learning journey by orchestrating the deployment of an ordering system. The `order-orchestrator` ties together the application (`order-service`) and infrastructure (`order-infra`) using Git submodules, providing a seamless deployment workflow.

## 🛠️ Tech Stack
- **Orchestration**: Git Submodules 📂
- **Deployment**: Bash scripts and Maven 📜
- **Application**:
  - Java 21 ☕
  - Spring Boot 3.2 🌱
  - AWS SDK for Java 📊
- **Infrastructure**:
  - AWS CDK 2.140 (Java) 🛠️
  - Java 17 ☕
  - Maven 📦
- **AWS Services**:
  - **DynamoDB**: Order storage 📊
  - **Lambda**: Order processing ⚡
  - **API Gateway**: REST endpoints 🌍
  - **IAM**: Secure permissions 🔒
  - **CloudWatch**: Monitoring 📈

## 🌐 AWS Resources (Managed)
- **DynamoDB Table**: `OrdersTable` for storing orders 📋
- **Lambda Function**: `OrderFunction` for processing orders ⚙️
- **API Gateway**: REST API for order operations 🌐
- **IAM Roles**: For secure access 🔐
- **CloudWatch Logs**: For monitoring 📊

## 📂 Repository Structure
```
order-orchestrator/
├── order-service/          # Git submodule for order-service
├── order-infra/            # Git submodule for order-infra
└── README.md
```

## 🏁 Getting Started
1. **Clone the repository with submodules**:
   ```bash
   git clone --recurse-submodules https://github.com/locngoduc/order-orchestrator.git
   ```
   If already cloned:
   ```bash
   cd order-orchestrator
   mvn validate  # Ensure submodules are initialized
   ```
2. **Install dependencies**:
   ```bash
   mvn install
   ```
3. **Deploy the system**:
   ```bash
   ./scripts/deploy.sh
   ```

## 🔗 Related Repositories
- **Application**: [order-service](https://github.com/locngoduc/order-service.git) (Java backend)
- **Infrastructure**: [order-infra](https://github.com/locngoduc/order-infra.git) (AWS CDK setup)

## 📚 Learning Goals
- Coordinate application and infrastructure deployment with Git submodules.
- Automate builds and deployments for AWS-based projects using Java.
- Understand the integration between Java apps and AWS infrastructure.

## 💡 Why This Impresses
- **End-to-End Workflow**: Combines Java app development with Java-based AWS CDK infrastructure.
- **Automation**: Streamlines deployment with a single command.
- **AWS Focus**: Leverages multiple AWS services for a real-world ordering system.

---

*Built with ⚙️ and ☁️ as a learning project for AWS mastery.*
