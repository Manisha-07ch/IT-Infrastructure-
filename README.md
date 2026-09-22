# 🖥️ Windows Server & MCSA Lab Projects

Welcome to my **Windows Server Infrastructure Lab Portfolio**.

This repository contains hands-on Windows Server projects that I implemented in a **VMware virtual lab environment**. The projects demonstrate practical skills in **Active Directory, DNS, DHCP, File Services, Group Policy, Backup & Restore, FSRM, DFS, RRAS VPN, networking, security, and troubleshooting**.

These projects are designed to demonstrate my practical understanding of Windows Server and IT Infrastructure concepts through configuration, testing, validation, and documentation.

---

## 👩‍💻 About Me

**Manisha Chaudhari**

Aspiring **IT Support / Network Engineer / Windows Server Administrator**

### Technical Areas

* Windows Server
* Active Directory
* DNS
* DHCP
* Networking Fundamentals
* VMware
* File and Print Services
* Group Policy
* NTFS & SMB Permissions
* Windows Server Backup
* FSRM
* DFS
* RRAS
* VPN
* Firewall
* Troubleshooting
* Basic Linux

---

# 🧪 Lab Environment

| Component          | Details                          |
| ------------------ | -------------------------------- |
| Virtualization     | VMware Workstation               |
| Server OS          | Windows Server 2016              |
| Client OS          | Windows Client                   |
| Domain Environment | Active Directory Domain Services |
| Network            | Virtualized Lab Network          |
| Project Type       | Hands-on Training / Lab          |

---

# 📂 Projects

## 1️⃣ MCSA-P01 — New Office Infrastructure

### Objective

Build a Windows Server infrastructure for a small business environment with centralized identity management, network services, controlled file access, Group Policy, backup, and recovery.

### Technologies

* Active Directory Domain Services
* DNS
* DHCP
* SMB
* NTFS Permissions
* Group Policy
* Windows Server Backup
* Windows Firewall
* Event Logs
* VMware

### Virtual Machines

```text
AST-DC01
AST-FS01
AST-BK01
AST-CL01
```

### Main Tasks

* Installed and configured Windows Server
* Configured Active Directory Domain Services
* Created domain environment
* Configured DNS
* Configured DHCP
* Created users and security groups
* Configured file shares
* Applied SMB and NTFS permissions
* Configured Group Policy
* Configured Windows Server Backup
* Performed restore testing
* Checked firewall and event logs
* Validated user access and network connectivity

### Evidence

📁 [View P01 Project](./P01-New-Office/)

---

# 2️⃣ MCSA-P02 — Controlled Document Centre

### Objective

Build a controlled document storage environment using file-server management, quotas, file screening, DFS Namespace, and DFS Replication.

### Technologies

* Windows Server
* SMB
* NTFS
* File Server Resource Manager (FSRM)
* Quotas
* File Screening
* DFS Namespace
* DFS Replication
* Windows Server Backup

### Virtual Machines

```text
AST-DC01
AST-FS01
AST-FS02
AST-BK01
AST-CL01
```

### Main Tasks

* Configured second file server
* Created file shares
* Configured FSRM
* Created storage quotas
* Configured file screening
* Configured DFS Namespace
* Added DFS targets
* Configured DFS Replication
* Tested replication/convergence
* Configured backup
* Performed restore validation

### Evidence

📁 [View P02 Project](./P02-Document-Centre/)

---

# 3️⃣ MCSA-P03 — Remote Employee Access

### Objective

Implement controlled remote access to internal resources using a Windows Server VPN environment.

The lab scenario includes remote access to internal resources while avoiding direct RDP exposure to the simulated WAN.

### Technologies

* RRAS
* VPN
* L2TP/IPsec
* Routing
* DNS
* SMB
* RDP
* Network Level Authentication
* Windows Firewall

### Main Tasks

* Configured RRAS
* Configured remote access VPN
* Configured L2TP over IPsec
* Configured routing and return paths
* Configured dial-in access
* Tested DNS over VPN
* Tested SMB access over VPN
* Configured RDP with NLA
* Configured firewall controls
* Tested authorized access
* Tested access revocation

### Evidence

📁 [View P03 Project](./P03-Remote-Access/)

---

# 🖧 Lab Architecture

```text
                         ┌─────────────────┐
                         │    AST-DC01     │
                         │ AD DS / DNS /   │
                         │      DHCP       │
                         └────────┬────────┘
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
             ┌──────▼──────┐             ┌──────▼──────┐
             │   AST-FS01  │             │   AST-FS02  │
             │ File Server │             │ FSRM / DFS  │
             │ SMB / NTFS  │             │ Replication │
             └──────┬──────┘             └─────────────┘
                    │
             ┌──────▼──────┐
             │   AST-CL01  │
             │    Client   │
             │   Testing   │
             └─────────────┘

                    Remote Access
                         │
                  ┌──────▼──────┐
                  │ Remote User │
                  │  RRAS VPN   │
                  │ L2TP/IPsec  │
                  └─────────────┘
```

---

# 🔐 Security & Access Control

The projects include practical configuration and validation of:

* User authentication
* Security groups
* NTFS permissions
* SMB permissions
* Group Policy
* Windows Firewall
* VPN authentication
* RDP Network Level Authentication
* Controlled remote access
* Access revocation
* Backup and restore

---

# 🧪 Testing & Validation

Each project includes validation of the configured services.

Examples include:

```text
✓ Domain connectivity
✓ DNS name resolution
✓ DHCP address assignment
✓ User authentication
✓ File-share access
✓ NTFS permission testing
✓ SMB permission testing
✓ Group Policy application
✓ Backup completion
✓ File restore
✓ DFS replication
✓ VPN connectivity
✓ Remote resource access
✓ Access revocation
```

Screenshots and supporting documentation are stored inside the individual project folders.

---

# 📸 Project Evidence

The repository contains screenshots showing the configuration and validation performed inside the VMware lab.

Example:

```text
P01-New-Office/
│
├── README.md
│
├── VMware/
├── Active-Directory/
├── DNS-DHCP/
├── File-Server/
├── Group-Policy/
├── Backup-Restore/
└── Validation/
```

---

# 🧰 Skills Demonstrated

### Windows Server

```text
Active Directory
DNS
DHCP
Group Policy
SMB
NTFS
Backup & Restore
Windows Firewall
Event Logs
```

### File Services

```text
FSRM
Quotas
File Screening
DFS Namespace
DFS Replication
```

### Networking

```text
IP Addressing
DHCP
DNS
Routing
VPN
RRAS
L2TP/IPsec
Network Troubleshooting
```

### Virtualization

```text
VMware Workstation
Virtual Machines
Virtual Networking
Windows Server Lab Environment
```

---

# 📚 What I Learned

Through these projects, I practiced:

* Building a Windows Server lab from virtual machines
* Deploying and managing Active Directory
* Managing users and security groups
* Configuring DNS and DHCP
* Managing SMB and NTFS permissions
* Applying Group Policy
* Implementing backup and restore
* Managing file-server storage
* Configuring FSRM and DFS
* Implementing remote-access VPN
* Troubleshooting connectivity and permissions
* Testing and documenting infrastructure configurations

---

# 🎯 Project Documentation Approach

For each project, I documented the following:

```text
1. Project Objective
        ↓
2. Lab Environment
        ↓
3. VMware Configuration
        ↓
4. Server Configuration
        ↓
5. Service Configuration
        ↓
6. Security / Permissions
        ↓
7. Testing
        ↓
8. Troubleshooting
        ↓
9. Validation
        ↓
10. Screenshots / Evidence
```

---

# 📁 Repository Structure

```text
MCSA-Windows-Server-Projects/
│
├── README.md
│
├── P01-New-Office/
│   ├── README.md
│   ├── VMware/
│   ├── Active-Directory/
│   ├── DNS-DHCP/
│   ├── File-Server/
│   ├── Group-Policy/
│   ├── Backup-Restore/
│   └── Validation/
│
├── P02-Document-Centre/
│   ├── README.md
│   ├── FSRM/
│   ├── DFS/
│   ├── File-Server/
│   ├── Backup-Restore/
│   └── Validation/
│
└── P03-Remote-Access/
    ├── README.md
    ├── RRAS/
    ├── VPN/
    ├── Routing/
    ├── Firewall/
    ├── RDP/
    └── Validation/
```

---

# 💼 Career Relevance

These projects demonstrate practical exposure to technologies commonly used in **IT Support, Windows Server Administration, Network Administration, and Infrastructure Support** environments.

They also demonstrate my ability to:

* Build a virtual lab
* Follow implementation requirements
* Configure infrastructure services
* Apply security controls
* Troubleshoot technical issues
* Test configurations
* Document technical work
* Present evidence of completed tasks

---

# 📌 Disclaimer

These are **hands-on training/lab projects** completed in a virtualized VMware environment.

They should not be interpreted as production employment experience or as proof of holding an earned MCSA certification.

The project documentation is intended to demonstrate practical learning, configuration skills, troubleshooting, and technical understanding.

---

# 📫 Contact

**Manisha Chaudhari**

Interested in opportunities related to:

* IT Support
* Network Support
* Windows Server Administration
* Network Engineering
* IT Infrastructure


