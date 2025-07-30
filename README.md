# ☁️ Azure VM Security Automation

This project demonstrates the **automated deployment of secure Azure Virtual Machines** using Azure CLI and PowerShell. It focuses on applying security best practices such as network hardening, identity protection, and post-deployment configuration.

---

## 🎯 Objective

- Automate secure Azure VM deployment using CLI
- Apply **NSG (Network Security Group)** rules to restrict inbound traffic
- Enforce best practices for user identity and VM configuration
- Enable monitoring & auto-shutdown policies for cost control

---

## 🛠️ Technologies Used

| Tool / Platform | Usage |
|-----------------|-------|
| Azure CLI       | VM provisioning and resource configuration |
| PowerShell      | Post-deployment hardening |
| Azure Portal    | For visualization & monitoring |
| Bash Scripting  | Automation wrapper scripts |
| NSG             | Network security controls |

---

## ⚙️ Features Implemented

- ✅ Create VM with SSH key login only
- ✅ Apply NSG rules: allow only ports 22 & 443 (block all else)
- ✅ Set strong admin username & random passwords
- ✅ Enable VM auto-shutdown and backup policy
- ✅ Tagging resources for visibility & audit
- ✅ Optional: MFA + Azure AD login

---

## 📁 Directory Structure

```
azure-vm-security-automation/
├── scripts/
│   ├── deploy_vm.sh
│   ├── secure_nsg_rules.ps1
│   └── monitoring_setup.ps1
├── screenshots/
├── outputs/
│   └── vm_config.json
└── README.md
```

---

## 🚀 Deployment Instructions

### 🔧 Prerequisites:
- Azure CLI installed (`az login`)
- A valid Azure subscription
- SSH public key generated

### 💻 Step-by-Step:

```bash
# Login to Azure
az login

# Create resource group
az group create --name SecureVMGroup --location eastus

# Deploy secure VM
bash scripts/deploy_vm.sh
```

> ⚠️ Custom PowerShell scripts available in `/scripts` for Windows VMs.

---

## 📸 Screenshots

> Add screenshots of:
- Azure Portal view
- NSG rule configuration
- CLI deployment logs
- Monitoring enabled (optional)

---

## ✅ Outcomes

| Security Layer | Implemented |
|----------------|-------------|
| NSG Firewall   | ✅ Restricted |
| SSH Hardening  | ✅ SSH key only |
| Azure AD       | ✅ Configured |
| MFA            | ✅ Optional |
| Monitoring     | ✅ Enabled |

---

## 📚 References

- [Azure CLI Docs](https://learn.microsoft.com/en-us/cli/azure/)
- [Azure Security Best Practices](https://learn.microsoft.com/en-us/security/)
- [NSG Configuration](https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)

---

## 🧠 Summary

This project demonstrates a **cloud-ready, secure-by-default approach** to VM provisioning.  
It’s ideal for DevSecOps, SOC teams, and anyone building secure infrastructure in Azure.

