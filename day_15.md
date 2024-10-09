# Date - 05 July 2024
# INTRUSION DETECTION AND PREVENTION SYSTEMS

# Day 15: Intrusion Detection and Prevention Systems
Today’s I focused on Intrusion Detection and Prevention Systems (IDPS), which are essential tools in modern cyber security defenses. I learned that these systems are designed to detect and potentially stop unauthorized access to networks, systems, or data. IDPS are divided into two main categories: Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS).

---

## Objective: 
To understand the fundamentals of Intrusion Detection and Prevention Systems (IDPS) their types, functionality, and how they help in identifying and preventing security threats.

---

## Introduction to IDPS
### Overview of IDPS:
- An Intrusion Detection and Prevention System (IDPS) is a network security technology designed to detect and respond to potential security threats, such as unauthorized access, malware, and other malicious activities.
- Intrusion Detection Systems (IDS)** focus on identifying suspicious or harmful activity and alerting the administrators, while Intrusion Prevention Systems (IPS) not only detect but also actively block the threats.

---

### Goal: 
To prevent unauthorized access and reduce the damage from security incidents.

---

## Types of Intrusions:
1. Network-based Intrusions: Unauthorized access, denial-of-service (DoS) attacks, and data exfiltration attempts.

2. Host-based Intrusions: Exploitation of vulnerabilities in the operating system or applications, malware infections, and privilege escalation.

3. Application-level Intrusions: Attacks targeting specific applications, such as SQL injections, cross-site scripting (XSS), or buffer overflow attacks.

---

## Types of IDPS and Their Functionality

### Types of IDPS:
1. Network-Based IDPS (NIDPS):
   - Monitors network traffic for suspicious activity, such as unauthorized data transmissions or attempts to exploit vulnerabilities.
   - Can be deployed at key points in the network (e.g., perimeter, gateway, or server) to monitor traffic in real-time.
   - Example: Snort, Suricata.

2. Host-Based IDPS (HIDPS):
   - Installed on individual devices (such as servers or workstations) to monitor the behavior of the operating system, applications, and users.
   - Can detect activity such as unauthorized access attempts, file integrity changes, and abnormal behavior on the host.
   - Example: OSSEC, Tripwire.

3. Hybrid IDPS:
   - Combines elements of both network-based and host-based systems to provide a more comprehensive security approach.
   - Monitors both network traffic and host activities, offering better visibility into potential threats.

### How IDPS Works:
### 1. Detection Methods:
   - **Signature-Based Detection**:
     - Compares network traffic or system behavior against known attack patterns (signatures). If a match is found, the system generates an alert.
     - **Pro**: Effective for known threats.
     - **Con**: Unable to detect new or unknown threats.

   - **Anomaly-Based Detection**:
     - Establishes a baseline of normal behavior (e.g., network traffic volume, user activities) and raises alerts when there are deviations from this baseline.
     - **Pro**: Can detect new, previously unknown attacks.
     - **Con**: May produce false positives due to harmless anomalies in behavior.

   - **Heuristic-Based Detection**:
     - Uses algorithms to detect suspicious behavior that may indicate an attack. It combines pattern recognition with machine learning and statistical analysis to identify threats.
     - **Pro**: Can identify suspicious activity even if it does not match known signatures.
     - **Con**: Requires regular updates and tuning to avoid false positives.

### 2. Prevention Methods**:
   - **Blocking Traffic**: If an intrusion is detected, the IPS can automatically block the suspicious traffic to prevent it from entering or spreading within the network.

   - **Preventing Access**: The IPS may also shut down unauthorized sessions or disconnect compromised hosts from the network to mitigate the attack.

---

## Best Practices for Using IDPS:
1. Regular Updates: Ensure the IDPS is regularly updated with the latest attack signatures, threat intelligence feeds, and vulnerability patches.

2. Tuning and Configuration: Regularly fine-tune the system to minimize false positives and ensure it provides accurate alerts without overwhelming administrators.

3. Log and Analyze Alerts: Maintain detailed logs of detected events and conduct regular analysis to identify patterns or potential vulnerabilities that need addressing.

4. Integration with Other Security Tools: Ensure the IDPS integrates with other security systems (such as firewalls, SIEM solutions, and antivirus software) to provide a more comprehensive security posture.

5. Scalability: Choose an IDPS solution that can scale with the growth of the network, ensuring continuous protection as the organization expands.

---

## Today's Learning Summary:
- Today’s session gave me a solid understanding of **Intrusion Detection and Prevention Systems (IDPS)** and their role in network security. I now understand how IDPS can detect and block a wide variety of security threats, such as unauthorized access, malware, and network intrusions.
- I learned about the different types of IDPS (network-based, host-based, and hybrid) and their respective methods of detection, including signature-based, anomaly-based, and heuristic-based detection.
- Additionally, I gained insights into best practices for configuring, maintaining, and integrating IDPS with other security tools to ensure comprehensive protection against threats.

---

## Reflection:
- Intrusion detection and prevention are vital components of a multi-layered security strategy. Understanding how to use an IDPS effectively can significantly enhance an organization’s ability to detect, prevent, and respond to security incidents in real-time.
- The session highlighted the importance of regular updates, accurate alerting, and integration with other security systems, which will be key when implementing IDPS in a real-world scenario. This knowledge will be valuable for securing both small and large networks in a professional setting.

