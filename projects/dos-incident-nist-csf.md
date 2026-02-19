# Network DoS Incident Response and Analysis Using NIST CSF

## Project Overview  
This case study documents the analysis of a network security incident using the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF). The objective was to assess a Denial of Service (DoS) attack, identify control gaps, and define security improvements aligned with NIST best practices. The project demonstrates structured incident analysis, risk-informed decision making, and the practical application of an industry-recognized framework in a SOC-relevant context.

---

## Organizational Context  
**Organization Type:** Multimedia services company providing web design, graphic design, and social media marketing to small businesses.  
**Operational Impact:** A network outage disrupted internal operations for approximately two hours, preventing access to critical network resources and affecting service delivery.

---

## Incident Summary  
- **Attack Type:** Denial of Service (DoS) via ICMP flood  
- **Attack Vector:** High-volume ICMP traffic admitted through an unconfigured firewall  
- **Systems Impacted:** Internal network services and shared resources  
- **Duration:** Approximately two hours  
- **Root Cause:** Firewall misconfiguration permitting unrestricted ICMP traffic  
- **Immediate Mitigation:**  
  - Blocked inbound ICMP traffic  
  - Temporarily suspended non-critical services  
  - Prioritized restoration of critical services  

---

## Analysis Aligned to the NIST Cybersecurity Framework (CSF)

### Identify  
- Confirmed malicious ICMP flood activity impacting the internal network.  
- Assessed the scope of impact across internal services and shared resources.  
- Identified firewall configuration weaknesses and limited pre-incident monitoring as primary contributors to service disruption.

### Protect  
- Implemented ICMP rate-limiting rules on the firewall to reduce exposure to volumetric traffic.  
- Deployed IDS/IPS controls to filter ICMP traffic exhibiting suspicious characteristics.  
- Established baseline firewall configuration standards to reduce future misconfiguration risk.

### Detect  
- Enabled source IP verification on firewall rules to identify spoofed traffic.  
- Implemented network monitoring to detect abnormal ICMP traffic patterns and availability-impacting events.  
- Defined alert thresholds to support timely identification of anomalous network behavior.

### Respond  
- Isolated affected services to contain the impact and prevent further disruption.  
- Restored critical services in accordance with operational priorities.  
- Conducted log review to identify indicators of abnormal activity and validate containment actions.  
- Documented the incident and communicated findings to stakeholders to support continuous improvement of response procedures.

### Recover  
- Restored services to normal operating conditions following traffic stabilization.  
- Reintroduced non-critical services after validation of network stability.  
- Documented recovery procedures and incorporated lessons learned into operational playbooks.

---

## Tools and Technologies  
- Network firewall (ICMP rate limiting, source IP verification)  
- Intrusion Detection/Prevention System (IDS/IPS)  
- Network monitoring and logging tools  
- NIST Cybersecurity Framework (CSF)

---

## Outcomes and Skills Demonstrated  
**Outcomes:**  
- Reduced exposure to ICMP flood attacks through firewall hardening and rate limiting  
- Improved detection of abnormal network traffic patterns  
- Established structured response and recovery processes for availability incidents  

**Skills Demonstrated:**  
- Incident analysis and documentation  
- Application of NIST CSF (Identify, Protect, Detect, Respond, Recover)  
- Network security hardening and control implementation  
- Operational prioritization during incident response  
- Post-incident review and process improvement

---

## Lessons Learned  
- Firewall configuration management is a critical control for mitigating network-layer attacks.  
- Proactive monitoring and traffic rate controls materially reduce the operational impact of DoS events.  
- A structured framework such as NIST CSF improves consistency and effectiveness in incident response and recovery.  
- Clear response and recovery procedures reduce service downtime and support business continuity.
