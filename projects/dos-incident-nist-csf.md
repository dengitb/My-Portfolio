# Network DoS / DDoS Incident Response and Analysis (NIST CSF)

## Incident / Assessment Overview  
This project documents the analysis of a network security incident in a simulated enterprise environment involving a Distributed Denial of Service (DDoS) attack. The organization experienced a service disruption when all internal network services suddenly stopped responding due to a flood of incoming ICMP packets. The incident impacted availability of critical network resources and required immediate containment and recovery actions.

The objective of this assessment was to analyze the incident using the **National Institute of Standards and Technology Cybersecurity Framework (NIST CSF)** and develop a structured response and improvement plan aligned with industry best practices.

---

## Technical Approach & Tools Used  

### Framework & Methodology  
The incident was analyzed using the five NIST CSF functions:  
- **Identify**  
- **Protect**  
- **Detect**  
- **Respond**  
- **Recover**

This framework was used to assess root cause, containment actions, and long-term security improvements.

### Technical Controls Implemented  
- Network firewall (ICMP rate limiting)  
- Source IP address verification on firewall rules  
- Intrusion Detection/Prevention System (IDS/IPS)  
- Network monitoring and logging tools  

### NIST CSF Mapping  

**Identify**  
A malicious actor (or actors) targeted the organization with an ICMP flood attack that disrupted the entire internal network. Critical network resources were impacted and required prioritization for restoration.

**Protect**  
The cybersecurity team implemented firewall rate-limiting rules for ICMP traffic and deployed IDS/IPS controls to filter malicious ICMP packets based on suspicious characteristics.

**Detect**  
Source IP address verification was configured on firewall rules to detect spoofed IP addresses. Network monitoring software was deployed to identify abnormal ICMP traffic patterns and availability-impacting events.

**Respond**  
Affected services were isolated to prevent further disruption. Non-critical services were taken offline to prioritize restoration of critical systems. Network logs were analyzed to identify indicators of attack activity, and the incident was documented and escalated to management for visibility and improvement planning.

**Recover**  
Critical network services were restored first to return essential business operations to normal. Non-critical services were reintroduced after traffic stabilized. Firewall rules were updated to block future ICMP flood attempts, and recovery procedures were documented for future incident handling.

---

## Key Findings & Impact  

### Key Findings  
- Firewall misconfiguration allowed unrestricted ICMP traffic into the network  
- Lack of ICMP rate limiting increased susceptibility to volumetric network attacks  
- Limited pre-incident monitoring reduced early detection capability  

### Impact  
- Complete disruption of internal network services  
- Temporary outage of critical business systems  
- Elevated operational risk due to availability failures  

These gaps significantly increased the organization’s exposure to denial-of-service attacks and business disruption.

---

## Lessons Learned & Security Improvements  

### Lessons Learned  
- Firewall configuration management is a critical control for mitigating network-layer attacks.  
- Proactive monitoring and traffic rate controls materially reduce the operational impact of DoS/DDoS events.  
- Applying a structured framework such as NIST CSF improves consistency, communication, and effectiveness in incident response.

### Security Improvements Implemented  
- Enforced ICMP rate limiting at the firewall  
- Deployed IDS/IPS to improve detection and filtering of malicious traffic  
- Implemented network monitoring to detect abnormal traffic patterns  
- Documented response and recovery procedures for availability incidents  

---

## Skills Demonstrated  
- Incident analysis using NIST Cybersecurity Framework (CSF)  
- Network security hardening and firewall rule design  
- IDS/IPS deployment and monitoring strategy  
- Incident response documentation and recovery planning  
- Availability risk assessment and mitigation
