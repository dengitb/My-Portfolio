#  Network DoS Incident Response & Analysis (NIST CSF)

##  Project Overview  
This project documents the analysis of a real-world–inspired network security incident using the **National Institute of Standards and Technology Cybersecurity Framework (NIST CSF)**. The objective was to assess a Denial of Service (DoS) attack, identify security gaps, and design security improvements aligned with NIST best practices. This case study demonstrates structured incident analysis, risk-based decision making, and alignment with industry frameworks commonly used in SOC and enterprise environments.

---

## Organizational Context  
**Organization Type:** Multimedia company providing web design, graphic design, and social media marketing services to small businesses.  
**Business Impact:** The internal network outage disrupted business operations and prevented employees from accessing network resources for approximately two hours, directly impacting service delivery to clients.

---

## Incident Summary  
- **Attack Type:** Denial of Service (DoS) / ICMP Flood (DDoS-style traffic)  
- **Attack Vector:** Flood of ICMP packets sent through an unconfigured firewall  
- **Systems Impacted:** Internal network services and resources  
- **Duration:** ~2 hours of service disruption  
- **Root Cause:** Firewall misconfiguration allowing unrestricted ICMP traffic  
- **Immediate Mitigation:**  
  - Blocked incoming ICMP packets  
  - Stopped non-critical network services  
  - Restored critical network services  

---

## NIST CSF–Aligned Analysis

### Identify  
**Risk & Asset Identification**
- Identified malicious ICMP flood attack targeting the internal network.  
- Determined that the entire internal network was impacted, affecting availability of business-critical services.  
- Identified firewall misconfiguration as the primary vulnerability enabling the attack.  
- Recognized lack of sufficient network monitoring and rate limiting as contributing factors.  

**Security Gaps Identified:**
- No ICMP rate limiting in place  
- Inadequate firewall configuration  
- Limited proactive monitoring for abnormal traffic patterns  

---

### Protect  
**Preventive Controls Implemented**
- Implemented firewall rules to **rate-limit incoming ICMP packets**.  
- Deployed **IDS/IPS controls** to filter ICMP traffic exhibiting suspicious patterns.  
- Hardened firewall configurations to reduce exposure to network-layer flooding attacks.  

**Additional Protective Recommendations:**
- Establish baseline firewall configuration standards  
- Implement network segmentation to limit blast radius of future attacks  
- Conduct routine firewall rule audits and configuration reviews  

---

### Detect  
**Detection Enhancements**
- Enabled **source IP address verification** on the firewall to detect spoofed IP addresses.  
- Implemented **network monitoring software** to identify abnormal traffic patterns and sudden spikes in ICMP activity.  

**Detection Strategy Improvements:**
- Define alert thresholds for ICMP rate anomalies  
- Integrate network monitoring alerts into a centralized logging or SIEM platform  
- Establish detection playbooks for volumetric network attacks  

---

### Respond  
**Incident Response Actions**
- Isolated affected network services to prevent further disruption.  
- Prioritized restoration of **critical services** to maintain essential business operations.  
- Conducted log analysis to identify indicators of abnormal or malicious network activity.  
- Reported the incident to management and documented response actions for accountability and post-incident review.  

**Response Process Improvements:**
- Develop formal DoS/DDoS response playbooks  
- Define clear communication channels between IT, security, and leadership  
- Conduct tabletop exercises to improve response readiness  

---

### Recover  
**Service Restoration**
- Restored network services to normal operation after attack traffic subsided.  
- Brought non-critical services back online after stabilizing critical systems.  

**Recovery Enhancements:**
- Documented recovery procedures for future network availability incidents  
- Established recovery priorities to minimize downtime in future events  
- Recommended post-incident review process to incorporate lessons learned into security controls  

---

## Tools & Technologies  
- Firewall (ICMP rate limiting, source IP verification)  
- IDS/IPS  
- Network monitoring tools  
- NIST Cybersecurity Framework (CSF)  

---

## Key Outcomes & Skills Demonstrated  
**Outcomes:**
- Improved firewall configuration to mitigate ICMP flood attacks  
- Enhanced visibility into abnormal network traffic patterns  
- Established structured response and recovery procedures  

**Skills Demonstrated:**
- Incident response planning and execution  
- Network security hardening  
- Application of NIST CSF (Identify, Protect, Detect, Respond, Recover)  
- Risk analysis and security control selection  
- Professional incident documentation and reporting  

---

## Lessons Learned  
- Firewall misconfigurations can enable simple yet highly disruptive network-layer attacks.  
- Proactive monitoring and rate limiting significantly reduce the impact of volumetric DoS attacks.  
- Using the NIST CSF provides a repeatable, structured methodology for improving security posture after incidents.  
- Clearly defined response and recovery procedures reduce downtime and operational impact during network outages.
