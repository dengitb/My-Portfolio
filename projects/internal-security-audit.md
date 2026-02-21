# Internal IT Security Audit & Compliance Review (Simulated Enterprise)

## Incident / Assessment Overview

This project presents an internal IT security audit conducted in a simulated enterprise environment based on a fictional organization, **Botium Toys**, a small U.S. toy manufacturer/retailer with one physical location (office, storefront, and warehouse) and a growing international e-commerce presence.

As online sales expanded, the organization faced increasing risk related to **payment processing, customer data protection, and regulatory compliance**. To address these risks, the IT manager initiated an **internal IT audit** to assess the organization’s current security posture, identify control gaps, and evaluate compliance readiness.

Before the audit began, the IT manager:
- Applied the **NIST Cybersecurity Framework (NIST CSF)** to guide the security program review  
- Defined the **audit scope and goals**  
- Documented the **assets managed by IT**  
- Completed a **risk assessment** to summarize potential risk exposure and possible fines  

**My role:** Review the IT manager’s scope, goals, and risk assessment report, then perform the internal audit by completing a **Controls and Compliance Checklist** to determine which controls and best practices were in place and which required improvement.

---

## Technical Approach & Tools Used

I began by reviewing the audit scope, goals, asset inventory, and risk assessment prepared by the IT manager:

- [Scope, Goals, Asset Inventory, and Risk Assessment Report](./artifacts/botium-toys-scope-goals-risk-assessment.md)
- [Scope, Goals, Asset Inventory, and Risk Assessment Report](https://docs.google.com/document/d/13VUAUTGZIhw9iAWh7tandFvTIW4C9yyjTgSFozs_EAE/edit?usp=sharing)

Key risk themes identified in the report included broad internal access to sensitive data, lack of encryption for payment data, missing access controls (least privilege and separation of duties), missing intrusion detection capabilities (IDS), and lack of backups and disaster recovery planning.

To ensure a consistent and structured review, I used industry-standard control categories (administrative, technical, and physical controls), aligned with common enterprise security and audit practices, to determine whether controls were present and where gaps existed:

- [Control Categories (Administrative, Technical, Physical)](./artifacts/control-categories.md)

Using these categories, I assessed controls as **preventative, detective, corrective, or deterrent**, then documented results in the audit checklist.

I performed the internal audit by completing the controls and compliance checklist based on evidence described in the risk assessment report:

- [Completed Controls and Compliance Checklist](./artifacts/controls-and-compliance-checklist.md)

This checklist captured whether key controls (e.g., encryption, IDS, backups, least privilege, password management) and compliance best practices (PCI DSS, GDPR, SOC trust principles) were currently met.

---

## Key Findings & Impact

### Control Gaps Identified

**Administrative / Managerial**
- No enforcement of least privilege  
- No separation of duties  
- Weak password policy enforcement  
- No centralized password management  
- No disaster recovery planning  

**Technical**
- Firewall and antivirus were present  
- No intrusion detection system (IDS)  
- No encryption for sensitive payment data  
- No backups for recovery  

**Physical / Operational**
- Locks, CCTV, and fire detection/prevention were present and provided baseline facility protection  

### Compliance Gaps

**PCI DSS**
- Inadequate restriction of access to cardholder data  
- Lack of encryption  
- Weak password management practices  

**GDPR**
- Breach notification planning existed  
- Asset classification and access controls required improvement  

**SOC (CIA Principles)**
- **Confidentiality:** Impacted by broad access and lack of encryption  
- **Availability:** Impacted by absence of backups and disaster recovery planning  

**Impact:**  
These gaps significantly increased the organization’s exposure to data breaches, ransomware incidents, operational downtime, and potential regulatory penalties.

---

## Lessons Learned & Security Improvements

### Lessons Learned
- Asset visibility and access control are foundational to reducing organizational risk  
- Detection and recovery capabilities (IDS, backups, DR) are critical for minimizing business impact during incidents  
- Security audits are most effective when findings are translated into prioritized, actionable remediation steps  

### Recommended Security Improvements
- Enforce least privilege and separation of duties  
- Encrypt payment card data and sensitive customer information  
- Deploy IDS for improved detection and monitoring  
- Implement regular backups and a formal disaster recovery plan  
- Strengthen and enforce password policies with centralized management  
- Formalize asset inventory and classification processes  

---

## Skills Demonstrated

- Internal IT audit execution using structured assessment checklists  
- Control evaluation across administrative, technical, and physical domains  
- Risk-based remediation prioritization  
- Compliance gap analysis (PCI DSS, GDPR concepts)  
- Professional security documentation and stakeholder-ready recommendations  
