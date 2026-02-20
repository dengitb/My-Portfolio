# Internal Security Audit & Compliance Assessment (Simulated Enterprise)

## Project Overview  
This case study documents an internal security audit conducted within a simulated enterprise environment to evaluate organizational security posture and compliance readiness. The objective was to review the audit scope and risk assessment, assess existing controls across administrative, technical, and physical domains, and identify compliance gaps related to payment card data and customer privacy. The final deliverable was a completed controls and compliance checklist with prioritized recommendations to reduce risk and improve business continuity.

---

## Organizational Context  
**Environment Type:** Simulated small business with a physical office, storefront, warehouse, and an expanding e-commerce presence serving domestic and international customers.  
**Business Challenge:** Rapid online growth increased pressure on IT operations to securely support e-commerce transactions while protecting customer data and maintaining operational continuity.  
**Audit Drivers:** Elevated risk of data exposure, service disruption, and regulatory or financial impact due to missing security controls and incomplete compliance practices.

---

## Audit Scope and Objectives  
**Scope:**  
- Employee devices and endpoints  
- Internal network and internet connectivity  
- Core business systems (e-commerce, databases, inventory, accounting)  
- Data storage and retention practices  
- Legacy systems requiring manual monitoring  
- Physical facilities (office, storefront, warehouse)  

**Objectives:**  
- Identify and categorize critical assets and exposure areas  
- Evaluate the presence and effectiveness of administrative, technical, and physical controls  
- Assess compliance readiness for payment security and data privacy obligations  
- Produce actionable, risk-prioritized recommendations to strengthen security posture

---

## Key Assets Reviewed  
- End-user devices and peripherals (desktops/laptops, smartphones, remote workstations)  
- Internal network infrastructure and internet access  
- Business applications and data stores (e-commerce platform, databases, inventory systems)  
- Sensitive customer data (payment information, PII)  
- Legacy systems requiring ongoing maintenance  
- Physical security controls protecting facilities and equipment

---

## Risk Snapshot  
- **Overall Risk Level:** High  
- **Primary Risk Factors:**  
  - Limited asset visibility and classification  
  - Broad internal access to sensitive data (payment data and PII)  
  - Lack of encryption for sensitive information  
  - Absence of least privilege and separation of duties  
  - Limited detection visibility due to missing IDS  
  - No formal backups or disaster recovery planning  
  - Weak password policy enforcement and no centralized password management  

- **Existing Baseline Controls:**  
  - Firewall filtering  
  - Antivirus protection  
  - Physical security measures (locks, CCTV, fire detection/prevention)  
  - Breach notification procedures aligned with privacy obligations

---

## Controls Assessment Summary  

### Administrative / Managerial Controls  
Identified gaps in least privilege enforcement, separation of duties, password policy strength, centralized password management, and disaster recovery planning. These weaknesses increase the likelihood and impact of account compromise, insider misuse, and prolonged operational disruption.

### Technical Controls  
Baseline protections (firewall, antivirus) were present; however, critical gaps were identified in intrusion detection, encryption of sensitive data, and backup mechanisms necessary for ransomware recovery and system restoration.

### Physical / Operational Controls  
Physical safeguards (locks, CCTV, fire detection/prevention) provided a reasonable baseline for facility protection, reducing the risk of unauthorized physical access to assets.

---

## Compliance Readiness Summary  

**Payment Security:**  
Identified gaps in restricting access to cardholder data, encrypting sensitive payment information, and enforcing secure password management practices.

**Data Privacy:**  
Breach notification processes existed, but improvements were needed in asset classification, access control enforcement, and confidentiality protections to reduce regulatory exposure.

**Confidentiality, Integrity, Availability (CIA):**  
- **Confidentiality:** Weakened by broad access and lack of encryption  
- **Integrity:** Partially supported through existing system controls  
- **Availability:** At risk due to lack of backups and disaster recovery planning

---

## Audit Artifacts & References  
The following artifacts were used to conduct the audit and document findings:

- **Audit Scope, Goals, and Risk Assessment Report**  
  → `./artifacts/scope-goals-risk-assessment.pdf`  

- **Control Categories (Administrative, Technical, Physical Controls)**  
  → `./artifacts/control-categories.pdf`  

- **Controls and Compliance Checklist (Completed Deliverable)**  
  → `./artifacts/controls-and-compliance-checklist.xlsx`  

> _Note: Artifact names and paths can be adjusted to match your repository structure._

---

## Recommendations (Prioritized)  
- Enforce least privilege and role-based access control for sensitive systems  
- Implement encryption for payment data and sensitive customer information  
- Establish regular backups and formal disaster recovery procedures  
- Deploy intrusion detection to improve threat visibility  
- Strengthen password policies and implement centralized password management  
- Formalize asset inventory, classification, and ownership processes  

---

## Outcomes and Skills Demonstrated  
**Outcomes:**  
- Identified critical security and compliance gaps affecting confidentiality, integrity, and availability  
- Produced a prioritized remediation plan to strengthen security posture and resilience  

**Skills Demonstrated:**  
- Internal security auditing and control evaluation  
- Risk analysis and prioritization  
- Compliance gap assessment (payment security and data privacy)  
- Security documentation and stakeholder-focused recommendations  

---

## Lessons Learned  
- Asset visibility and access control are foundational to reducing organizational risk.  
- Detection and recovery capabilities are essential to minimizing operational impact during incidents.  
- Translating audit findings into prioritized, actionable recommendations is critical for improving real-world security posture.
