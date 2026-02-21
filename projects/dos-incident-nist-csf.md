# Network DoS Incident Response and Analysis (NIST CSF)

## Incident / Assessment Overview  
This case study documents the analysis and response to a network Denial of Service (DoS) incident using the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF). The objective was to assess the impact of an ICMP flood attack, identify control gaps, and define security improvements aligned with NIST best practices. The incident disrupted internal network services for approximately two hours, impacting business operations and service delivery.

**Organization Type:** Multimedia services company providing web design, graphic design, and social media marketing to small businesses.  

**Incident Summary:**  
- **Attack Type:** Denial of Service (DoS) via ICMP flood  
- **Attack Vector:** High-volume ICMP traffic allowed through an unconfigured firewall  
- **Systems Impacted:** Internal network services and shared resources  
- **Duration:** ~2 hours  
- **Root Cause:** Firewall misconfiguration permitting unrestricted ICMP traffic  

---

## Technical Approach & Tools Used  
I analyzed the incident using the **NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)** to structure response actions and remediation planning:

- **Identify:** Confirmed ICMP flood activity, assessed impact to internal services, and identified firewall configuration weaknesses and limited pre-incident monitoring.  
- **Protect:** Implemented ICMP rate limiting on the firewall and established baseline firewall configuration standards.  
- **Detect:** Enabled source IP verification and network monitoring to identify spoofed traffic and abnormal ICMP patterns.  
- **Respond:** Isolated affected services, restored critical systems first, reviewed logs for indicators of abnormal activity, and documented response actions.  
- **Recover:** Restored services to normal operations, validated network stability, and updated recovery procedures and response playbooks.

**Tools & Technologies:**  
- Network firewall (ICMP rate limiting, source IP verification)  
- IDS/IPS  
- Network monitoring and logging tools  
- NIST Cybersecurity Framework (CSF)

---

## Key Findings & Impact  
**Key Findings:**  
- Firewall misconfiguration significantly increased exposure to volumetric network-layer attacks.  
- Limited detection and monitoring delayed early identification of abnormal ICMP traffic.  
- Lack of predefined traffic rate controls increased the operational impact of the attack.

**Impact:**  
- Internal network services were unavailable for approximately two hours.  
- Business operations and service delivery were disrupted.  
- Incident response processes were ad hoc prior to formal documentation and playbook updates.

---

## Lessons Learned & Security Improvements  
**Lessons Learned:**  
- Firewall configuration management is a critical control for mitigating network-layer attacks.  
- Proactive monitoring and traffic rate controls materially reduce the operational impact of DoS events.  
- A structured framework such as NIST CSF improves consistency and effectiveness in incident response and recovery.

**Security Improvements Implemented / Recommended:**  
- Enforce firewall configuration baselines and change management procedures  
- Implement ICMP rate limiting and traffic filtering by default  
- Strengthen network monitoring and alert thresholds for abnormal traffic patterns  
- Maintain documented incident response and recovery playbooks to reduce downtime  
- Periodically test DoS response procedures through tabletop or simulated exercises  
