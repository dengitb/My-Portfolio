# 🚨 Network DoS Incident Analysis Using NIST CSF

## 📌 Overview  
This case study documents the analysis of a Denial of Service (DoS) network incident using the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF). The objective was to evaluate a real-world network security event and develop security improvements aligned with NIST best practices.

---

## 🏢 Scenario  
A multimedia company providing web design, graphic design, and social media marketing services experienced a network outage caused by a flood of ICMP packets. The attack disrupted internal network services for approximately two hours. The root cause was an unconfigured firewall that allowed excessive ICMP traffic, resulting in a DoS condition.

---

## 🔍 Incident Summary  
- **Attack Type:** Denial of Service (ICMP Flood / DDoS)  
- **Impact:** Internal network services became unavailable  
- **Root Cause:** Unconfigured firewall allowing ICMP packet flooding  
- **Initial Response:** ICMP traffic blocked; non-critical services stopped; critical services restored  

---

## 🧠 Analysis Using NIST Cybersecurity Framework (CSF)

### 🆔 Identify  
- Identified a malicious actor launching an ICMP flood attack.  
- Determined that the entire internal network was affected.  
- Recognized the firewall misconfiguration as a critical security gap.

### 🛡 Protect  
- Implemented firewall rules to limit the rate of incoming ICMP packets.  
- Deployed IDS/IPS to filter suspicious ICMP traffic.  

### 👁 Detect  
- Configured source IP address verification on the firewall to detect spoofed packets.  
- Implemented network monitoring software to detect abnormal traffic patterns.

### 🚑 Respond  
- Isolated affected systems to prevent further network disruption.  
- Restored critical services first to minimize operational impact.  
- Analyzed network logs for indicators of compromise.  
- Established escalation and reporting procedures to management and legal stakeholders.

### 🔄 Recover  
- Restored network services to normal operating state.  
- Prioritized restoration of critical services before non-essential services.  
- Implemented firewall-based ICMP filtering to prevent recurrence of similar attacks.

---

## 🧰 Tools & Technologies  
- Firewall (ICMP rate limiting, source IP verification)  
- IDS/IPS  
- Network monitoring software  
- NIST Cybersecurity Framework (CSF)

---

## 📈 Key Takeaways  
- Proper firewall configuration is critical to preventing basic network-layer attacks.  
- Rate limiting and IDS/IPS significantly reduce the impact of ICMP flood attacks.  
- Applying the NIST CSF provides a structured and effective approach to incident analysis and security improvement.  
- Proactive detection and response planning improves organizational resilience against network-based attacks.
