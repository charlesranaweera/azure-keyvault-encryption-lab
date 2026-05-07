# Azure Encryption Lab using Key Vault (Customer-Managed Keys)

## Overview

This hands-on lab demonstrates how to use Azure Key Vault customer-managed keys (CMK) to encrypt:

1. Azure Virtual Machine disks  
2. Azure Storage Account data

The objective was to strengthen cloud data protection and understand enterprise-grade encryption controls.

---

## Technologies Used

- Microsoft Azure
- Azure Key Vault
- Azure Virtual Machines
- Azure Managed Disks
- Azure Storage Account
- Customer-Managed Keys (CMK)

---

## Lab Part 1: VM Disk Encryption

### Steps Completed

1. Created Azure Key Vault
2. Generated RSA encryption key
3. Created Windows Server VM
4. Connected via RDP
5. Mounted new data disk
6. Enabled encryption for:
   - OS Disk
   - Data Disk
7. Verified successful encryption

### Result

Encrypted disks displayed lock icon in Azure portal.

---

## Challenges & Fixes

### Access Issue

Problem:
VM unable to access Key Vault.

Resolution:
- Allowed trusted Microsoft services
- Added authorised IP through firewall rules

### Key Size Compatibility

Used RSA 3072+ key size for newer Windows workloads.

---

## Lab Part 2: Storage Account Encryption

### Steps Completed

1. Created Storage Account
2. Selected Customer-Managed Key encryption
3. Linked Key Vault key
4. Validated encryption settings

---

## Security Benefits

- Full control over encryption keys
- Stronger compliance posture
- Centralised key lifecycle management
- Key rotation capability
- Improved governance

---

## Skills Demonstrated

Azure Security | Key Management | Encryption | Cloud Governance | Data Protection | Security Engineering
