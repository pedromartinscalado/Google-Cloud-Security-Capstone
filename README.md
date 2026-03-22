# Google Cloud Security: Data Breach Response & Remediation

## 📌 Project Overview
This project showcases the end-to-end incident response and infrastructure hardening performed for **Cymbal Retail** during a simulated data breach. I successfully remediated high-severity vulnerabilities and achieved **100% compliance with PCI DSS 3.2.1 standards**.

## 🛡️ Technical Implementation

### 1. Incident Response (NIST Framework)
* **Containment:** Restricted SSH access via Identity-Aware Proxy (IAP) and shut down compromised instances.
* **Eradication:** Removed malware-infected VMs and deleted permissive "allow-all" firewall rules.
* **Recovery:** Restored services using secure Compute Engine snapshots with **Secure Boot** enabled.

### 2. Infrastructure Hardening
* **Identity-Aware Proxy (IAP):** Eliminated public IP dependencies for administrative access.
* **Cloud Storage Security:** Converted buckets to **Uniform Access** and revoked all public permissions (`allUsers`).
* **VPC Firewall Logging:** Enabled comprehensive logging for internal traffic to detect lateral movement.

### 3. Compliance & Monitoring
* Utilized **Security Command Center (SCC)** to identify and fix vulnerabilities.
* Mitigated findings: *Open SSH/RDP ports*, *Public Bucket ACLs*, and *Malware communication*.

## 🛠️ Tools Used
* **Cloud Provider:** Google Cloud Platform (GCP)
* **Security Tools:** Security Command Center, Firewall Policies, IAM.
* **Compute:** Compute Engine (Hardening & Snapshots).
* **Storage:** Cloud Storage (Bucket Security), BigQuery (Data Protection).
