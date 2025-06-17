# 🚀 terraform-eks

> **A step-by-step, hands-on guide for deploying AWS EKS clusters with Terraform — perfect for learners and DevOps practitioners!**

---

## 🌟 What is this Project?

This repository provides an easy, practical way to create and manage Kubernetes clusters (EKS) on AWS using Terraform.  
You'll learn how to write, initialize, and apply Terraform code to automate the entire EKS provisioning process.

---

## 📂 Repository Structure

```plaintext
terraform-eks/
└── EKS-Deployment/
    ├── main.tf
    ├── variables.tf
    ├── outputs.tf
    ├── provider.tf
    └── README.md
```

---

## 🧑‍💻 Quick Start

### 1. **Set Up Terraform**

- Make sure you have Terraform installed.  
  Need help? [Follow this guide.](https://github.com/saifeezibrahim/DevOps-Tools-Installations/blob/main/DevOps-Tools-Installations-main/Terraform/terraform.sh)

### 2. **Clone this Repository**

```bash
git clone https://github.com/saifeezibrahim/terraform-eks.git
cd terraform-eks/terraform-eks/EKS-Deployment
```

### 3. **Initialize Terraform**

```bash
terraform init
```

### 4. **Validate the Configuration**

```bash
terraform validate
```

### 5. **Preview Infrastructure Changes**

```bash
terraform plan
```

### 6. **Apply the Changes**

```bash
terraform apply
```

### 7. **Update kubeconfig to Connect to EKS**

```bash
aws eks --region <your-region> update-kubeconfig --name <your-eks-cluster-name>
```
_Example:_
```bash
aws eks --region us-east-1 update-kubeconfig --name bankapp-eks-cluster
```

### 8. **Verify the Cluster Connection**

```bash
kubectl get nodes
```

---

## 🎓 What You'll Learn

- Real-world Infrastructure as Code (IaC) with Terraform
- Modular, reusable .tf files (main.tf, variables.tf, outputs.tf, etc.)
- EKS provisioning best practices
- Automating kubeconfig and cluster access
- The basics of cloud-native Kubernetes on AWS

---

## 💡 Tips

- Feel free to explore and modify the variables in `variables.tf` to customize your EKS cluster.
- Check out [AWS EKS Documentation](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) for extra learning.
- Try deploying sample Kubernetes apps to your new cluster!

---

## 🙋‍♂️ Maintained by Saifeez Ibrahim

If you found this helpful, star ⭐ the repo or share it to help more people learn DevOps!

Need help or want to connect? [Reach out on GitHub!](https://github.com/saifeezibrahim)

---

## 📄 License

MIT — Free to use for personal and educational purposes.

---

> **Happy automating and containerizing!**
