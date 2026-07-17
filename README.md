# DC-01 Base Operating System & Network Setup

## Virtual Machine Specifications
* **Operating System:** Windows Server (Base OS Deployment)
* **MAC Address:** 08:00:27:C8:85:A6

## Network Configuration
* **Hostname:** DC-01
* **IP Address:** 10.0.2.10
* **Subnet Mask:** 255.255.255.0
* **Gateway:** 10.0.2.2
* **DNS Server:** 127.0.0.1 (Loopback for Active Directory Services)

## Deployment Snapshot Strategy
To ensure environment stability and roll-back capability during the Active Directory build, the following virtual machine snapshots were executed:

1. `Clean_Base_OS_Installed`
   * **Description:** Fresh OS setup completed, hostname changed to DC-01, static network configuration verified, and permanent MAC address locked. No server roles added.
2. `Pre_Domain_Promotion`
   * **Description:** Active Directory Domain Services (AD DS) binaries successfully installed via Server Manager. System prepared and saved immediately prior to forest/domain creation.
  
