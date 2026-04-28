# NIST CSF Action Plan: Botium Toys Portfolio Artifact
**Analyst:** Arthur Sousa  
**Classification:** Internal Security Document  
**Framework Mapping:** NIST CSF v1.1

---

## 1. IDENTIFY (Asset & Risk Governance)
**Objective:** Develop the organizational understanding to manage cybersecurity risk to systems, assets, data, and capabilities.

*   **Cloud & Physical Asset Management:** Established a comprehensive inventory of storefront legacy systems, warehouse management databases, and global e-commerce cloud instances.
*   **Risk Assessment Modeling:** Utilized analytical logic to quantify the impact of unencrypted PII on organizational data sovereignty.
*   **Strategic Prioritization:** Identified high-value targets (HVT), prioritizing the credit card processing environment (CDE) as the primary security focus.

## 2. PROTECT (Security Safeguards)
**Objective:** Develop and implement appropriate safeguards to ensure delivery of critical infrastructure services.

*   **IAM Hardening:** Initiated a transition to a **Zero-Trust architecture**, enforcing the **Principle of Least Privilege (PoLP)** and Multi-Factor Authentication (MFA) across all administrative accounts.
*   **Encryption Standards:** Mandated **AES-256** for data-at-rest and **TLS 1.3** for data-in-transit, directly addressing GDPR Article 32 requirements.
*   **Network Micro-segmentation:** Designed a roadmap for segmenting e-commerce traffic from internal corporate assets via hardened pfSense firewall rules.

## 3. DETECT (Security Continuous Monitoring)
**Objective:** Develop and implement appropriate activities to identify the occurrence of a cybersecurity event.

*   **Intrusion Detection (IDS):** Strategized the deployment of cloud-native IDS nodes (Suricata/Snort) to monitor for malicious probes and SQL injection attempts.
*   **SIEM Integration:** Centralized telemetry and log data into an **ELK Stack (Elasticsearch, Logstash, Kibana)** dashboard for real-time threat hunting and alerting.

## 4. RESPOND (Incident Management)
**Objective:** Develop and implement appropriate activities to take action regarding a detected cybersecurity incident.

*   **Containment Playbooks:** Formulated technical steps for isolating compromised cloud instances to prevent lateral movement within the network.
*   **Escalation Matrix:** Defined a clear communication hierarchy (SOC Analyst ➔ SecOps Lead ➔ IT Management) to ensure rapid response times.
*   **Impact Analysis:** Established a post-detection procedure to determine the extent of data exfiltration during an active breach.

## 5. RECOVER (Resilience & Restoration)
**Objective:** Develop and implement appropriate activities to maintain plans for resilience and to restore impaired services.

*   **Disaster Recovery (DRP):** Drafted a formal plan focusing on meeting low **RTO (Recovery Time Objective)** and **RPO (Recovery Point Objective)** targets.
*   **Resilient Architecture:** Implemented automated daily snapshots and cross-region immutable backups for critical customer databases.
*   **Continuous Improvement:** Established a "Lessons Learned" protocol to update security policies and technical controls after every tabletop exercise or incident.
