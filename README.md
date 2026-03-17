# web-traffic-investigation
Web traffic analysis and incident investigation using Wireshark to detect SQL injection attack and compromise.

Web Traffic Investigation – SQL Injection Attack

This project presents a cybersecurity investigation of a web server compromise using network traffic analysis.

##  Overview
Analyzed captured network traffic using Wireshark to identify malicious activity targeting a web application. The investigation focused on detecting SQL Injection attempts, identifying attacker behavior, and reconstructing the attack timeline.

##  Objectives
- Identify the attack vector  
- Detect SQL Injection patterns  
- Analyze HTTP traffic  
- Extract attacker credentials  
- Determine if a system compromise occurred  

##  Tools Used
- Wireshark  
- CyberChef  

## Key Findings
- Attacker IP: **111.224.250.131**  
- Attack Method: **SQL Injection**  
- Exploited File: **search.php**  
- Compromised Credentials: **admin:admin123!**  
- Malicious File Uploaded: **NVri2vhp.php**  
- Unauthorized Access to: **/admin/**  

##  Attack Timeline
- Initial connection to web server  
- SQL Injection attempts using `UNION SELECT`  
- Database enumeration via INFORMATION_SCHEMA  
- Discovery of admin panel  
- Successful login using stolen credentials  
- Upload of malicious web shell  

## Conclusion
The investigation confirmed a successful SQL Injection attack that resulted in database enumeration, credential compromise, and remote code execution through a malicious file upload.

##  Recommendations
- Implement input validation and parameterized queries  
- Deploy Web Application Firewall (WAF)  
- Enforce strong password policies  
- Restrict access to sensitive directories  
- Monitor logs and detect suspicious activity  


Source: https://cyberdefenders.org/blueteam-ctf-challenges/web-investigation/

---

 This project demonstrates practical SOC analysis skills including network traffic analysis, incident response, and threat detection.
