# Internal IT Security Audit & Compliance Review (Simulated Enterprise)

## Scenario Context  
This project is based on a fictional organization, **Botium Toys**, a small U.S. toy manufacturer/retailer with one physical location (office, storefront, and warehouse) and a growing international e-commerce presence. As online sales expanded, the IT department faced increasing pressure to support global customers while maintaining secure payment processing and protecting customer data.

To address compliance and operational risk, the IT manager initiated an **internal IT audit**. Before the audit work began, the IT manager:
- Applied the **NIST Cybersecurity Framework (NIST CSF)** to guide the security program review  
- Defined the **audit scope and goals**  
- Documented the **assets managed by IT**  
- Completed a **risk assessment** to summarize potential risk exposure and possible fines related to gaps in controls and compliance

**My task:** Review the IT manager’s scope, goals, and risk assessment report, then perform the internal audit by completing a **Controls and Compliance Checklist** to determine which controls and best practices were in place and which required improvement.

---

## Project Overview  
This case study documents the internal audit work I performed after reviewing the IT manager’s documentation. The objective was to evaluate control coverage across **administrative/managerial**, **technical**, and **physical/operational** domains, and assess compliance readiness for:
- **Payment card data protection** (PCI DSS)
- **Customer privacy obligations** (GDPR)
- **Security trust principles** (SOC concepts: confidentiality, integrity, availability)

The final deliverable was a **completed controls and compliance checklist** with prioritized security recommendations.

---

## Inputs Reviewed (Provided by IT Manager)  
I began by reviewing the audit scope, goals, asset inventory, and risk assessment prepared by the IT manager:

- <a href="./artifacts/botium-toys-scope-goals-risk-assessment.md">Scope, Goals, Asset Inventory, and Risk Assessment Report</a>

Key risk themes identified in the report included broad internal access to sensitive data, lack of encryption for payment data, missing access controls (least privilege / separation of duties), missing IDS, and lack of backups/disaster recovery planning.

---

## Audit Method (How I Performed the Assessment)  
To ensure a consistent and structured review, I used industry-standard control categories (administrative, technical, and physical controls), aligned with common enterprise security and audit practices, to determine whether controls were present and where gaps existed:

- <a href="./artifacts/control-categories.md">Control Categories (Administrative, Technical, Physical)</a>

Using these categories, I assessed controls as preventative, detective, corrective, or deterrent, then documented results in the audit checklist.

---

## Primary Deliverable (Audit Checklist Completed)  
I performed the internal audit by completing the controls and compliance checklist based on evidence described in the risk assessment report:

- <a href="./artifacts/controls-and-compliance-checklist.md">Completed Controls and Compliance Checklist</a>

This checklist captured whether key controls (e.g., encryption, IDS, backups, least privilege, password management) and compliance best practices (PCI DSS/GDPR/SOC concepts) were currently met.

---

## Summary of Findings  

### Controls — High-Level Results  
- **Administrative/Managerial:** Gaps in least privilege, separation of duties, password policy strength/enforcement, centralized password management, and disaster recovery planning  
- **Technical:** Firewall and antivirus were present, but gaps existed in IDS, encryption for sensitive data, and backups  
- **Physical/Operational:** Locks, CCTV, and fire detection/prevention were present and provided a baseline level of facility protection  

### Compliance — High-Level Results  
- **PCI DSS:** Gaps in restricting access to cardholder data, securing storage/processing environments, encryption, and password management practices  
- **GDPR:** Breach notification planning existed, but improvements were needed in data classification/inventory and access controls to better protect EU customer data  
- **SOC Concepts (CIA):** Confidentiality and availability were most impacted due to broad access, lack of encryption, and lack of backups/DR planning

---

## Recommendations (Prioritized)  
- Implement least privilege and separation of duties for systems handling payment data and PII  
- Encrypt stored/processed payment card data and sensitive customer information  
- Deploy IDS to improve detection and monitoring capability  
- Establish backups and a disaster recovery plan to support business continuity  
- Strengthen password policy requirements and enforce them with centralized password management  
- Formalize asset inventory and classification to reduce unknown exposure

---

## Skills Demonstrated  
- Internal IT audit execution using a structured checklist  
- Control evaluation across administrative, technical, and physical domains  
- Risk-based prioritization of remediation actions  
- Compliance gap analysis (PCI DSS, GDPR)  
- Clear security documentation and stakeholder-ready recommendations
