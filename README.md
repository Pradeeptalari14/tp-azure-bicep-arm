# Azure Bicep/ARM Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure Bicep/ARM Studio** dashboard module.

## 🚀 Description
Design modular declarative configurations for Azure. Generate Bicep templates, nested parameter configuration files, and target resource group scopes definitions.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/bicep/main.bicep`
- **Execution Command**: `az deployment group create --resource-group rg --template-file main.bicep`
- **Validation Command**: `az deployment group list --resource-group rg`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-bicep-arm.git
   cd tp-azure-bicep-arm
   ```

2. **Run Execution Target:**
   ```bash
   az deployment group create --resource-group rg --template-file main.bicep
   ```

3. **Verify Runtime Stability:**
   ```bash
   az deployment group list --resource-group rg
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
