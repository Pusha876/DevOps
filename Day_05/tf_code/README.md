# 🌩️ Terraform Azure Pipeline Guide

Welcome to the **tf_code** folder!  
Here, you’ll find everything you need to **build, test, and deploy** Azure infrastructure using Terraform — all with a DevOps twist! 🚀

---

## 📁 Folder Structure

```
tf_code/
├── main.tf                   # Main Terraform configuration
├── variables.tf              # Input variables
├── outputs.tf                # Output values
├── terraform.tfstate         # Terraform state (not tracked in git)
├── terraform.tfstate.backup  # State backup (not tracked in git)
├── .terraform/               # Provider plugins & modules (not tracked in git)
├── .gitignore                # Git ignore rules
└── ...
```

---

## 🛠️ Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) installed
- [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli) installed & authenticated
- An Azure subscription with Contributor or Owner permissions

---

## 🚦 Quick Start: Terraform Workflow

### 1️⃣ **Initialize Terraform**
Get your environment ready and download providers.
```bash
terraform init
```

---

### 2️⃣ **Format & Validate**
Keep your code clean and error-free!
```bash
terraform fmt
terraform validate
```

---

### 3️⃣ **Plan the Magic**
Preview what Terraform will do before it does it.
```bash
terraform plan
```

---

### 4️⃣ **Apply the Changes**
Deploy your infrastructure to Azure!
```bash
terraform apply
```
_Confirm with `yes` when prompted._

---

### 5️⃣ **Check the State**
See what’s been created or changed.
```bash
terraform show
```

---

### 6️⃣ **Destroy (Optional)**
Tear down everything when you’re done.
```bash
terraform destroy
```
_Confirm with `yes` when prompted._

---

## 🔒 Security & Best Practices

- **Never commit sensitive files** like `secrets.txt` or `terraform.tfstate` to git.
- `.gitignore` is set up to keep your repo clean and safe.
- Always review your plan before applying changes.
- Use remote state (like Azure Storage) for team collaboration.

---

## 💡 Pro Tips

- Use different state files for dev, staging, and prod.
- Leverage variables and outputs for flexibility.
- Automate with Azure DevOps Pipelines for true CI/CD power!

---

## 🎉 Happy Terraforming!