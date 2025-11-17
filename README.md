#  Windows Server 2019: Enterprise Security Infrastructure Project

## Project Overview: The Zero-Trust Windows Defender Narrative

This repository documents the deployment and configuration of core Windows Server 2019 roles, focusing on **security hardening, attack surface minimization, and identity fortification**. This is not a basic setup; it's the implementation of a resilient, highly auditable enterprise foundation designed to meet modern security baselines.

### 1. Minimal Attack Surface & Hardening

My proficiency begins with fundamental hardening techniques to reduce the attack surface immediately upon deployment:

* **Server Core Implementation:** Prioritizing the **Normal Server (Server Core)** installation option for critical infrastructure roles (like Domain Controllers) to ensure the least resource-intensive environment with minimal software exposure.
* **Host-Level Network Control:** Configuring precise **Firewall rules** and secure network settings during initial installation, ensuring only essential protocols like **Remote Desktop** are allowed under strict conditions, embodying a **Zero-Trust principle** at the host level.
* **Secure Infrastructure Services:** Implementing core networking services (**DHCP** and **DNS**) with a security-first mindset, including securing **Dynamic DNS Updates** and creating **Reverse Lookup Zones** critical for proper auditing and rapid forensic investigation.

### 2. Identity and Access Control Fortification

I specialize in securing the most critical enterprise asset: the directory service.

* **Domain Controller Hardening:** Experienced in promoting servers to **Active Directory Domain Controllers** and configuring this core service to serve as a highly resilient and secure **root of trust** for all domain operations.
* **Virtualization-Based Security (VBS) Readiness:** Familiar with advanced security architecture, including the use of **Host Guardian support** and **Shielded VMs** (Datacenter Edition features), demonstrating an understanding of protecting high-value virtual machines from a compromised virtualization fabric.

### 3. Secure and Auditable Remote Management

I deploy management techniques that minimize exposure and maximize oversight.

* **Modern Secure Administration:** Utilizing **Windows Admin Center (WAC)**, a browser-based, modern management gateway, which relies on **WinRM with PowerShell Remoting and WMI** over secure channels for centralized, auditable control.
* **Centralized Monitoring:** Leveraging **Server Manager** for **multi-server management**, focusing on the **Events** and **Services** monitoring dashboards to proactively triage security alerts and track unauthorized changes.

---

## Technical Documentation Files

The following files document the step-by-step process of installation and configuration:

* `installation of the server 1.pptx` (Covers Server Core vs. GUI, Datacenter features like Shielded VMs)
* `initial installation 2.pptx` (Covers Firewall Rules and Remote Desktop setup)
* `promote a domain controller 3.pptx` (Details Active Directory Domain Services deployment)
* `manage server with server manager 4.pptx` (Covers multi-server management and event monitoring)
* `manage server with windows admin 5.pptx` (Details secure, browser-based management using WAC)
* `configure dns 6.pptx` (Covers Reverse Lookup Zone creation)
* `dhcp configurations 7.pptx` (Covers DHCP scope creation and Dynamic DNS Update configuration)
* `configure dhcp on server core11.pptx` (Covers DHCP on a minimal install environment)
