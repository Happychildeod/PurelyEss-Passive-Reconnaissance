# Passive Reconnaissance and OSINT Report – PurelyEss.com

### Author
Emmanuel Oladeinde  
Cybersecurity Analyst | Defensive and Reconnaissance Specialist

---

## Project Overview
This repository contains a passive reconnaissance assessment of the domain **PurelyEss.com**, performed in **November 2025**.  
The goal was to identify publicly available intelligence about the target domain using ethical OSINT techniques only.  
No intrusive or exploitative actions were conducted.

---

## Objectives
- Map the domain’s public exposure surface.  
- Identify registrar, DNS, and WAF/CDN configurations.  
- Verify presence of DNSSEC, SPF, DKIM, DMARC, and HTTP security headers.  
- Detect any credential leaks or exposure across public sources.

---

## Tools and Frameworks Used
| Category | Tool or Source | Purpose |
|-----------|----------------|----------|
| Domain and WHOIS | whois, rdap | Registration and expiration details |
| DNS Enumeration | dig, dnsrecon | Identify A/AAAA, NS, MX, TXT, and CAA records |
| WAF Detection | wafw00f | Detect CDN or WAF infrastructure |
| OSINT Automation | SpiderFoot (passive mode) | Subdomain and credential discovery |
| Banner and Header Review | Wapiti | Web header fingerprinting |
| OSINT References | OSINT Framework | CT logs, paste sites, and reputation sources |

---

## Key Findings
- The domain is hosted on the **Shopify CDN (23.227.38.32)**, providing built-in WAF and DDoS protection.  
- **DNSSEC** is not enabled.  
- Missing security headers (**HSTS, CSP, Referrer-Policy**).  
- No exposed credentials or sensitive data detected in passive OSINT sources.

Overall Exposure Rating: Low to Moderate

---

## Recommendations
1. Enable DNSSEC at the registrar level (GoDaddy).  
2. Implement security headers (HSTS, CSP, Referrer-Policy, Permissions-Policy).  
3. Configure SPF, DKIM, and DMARC for email authentication.  
4. Maintain CDN/WAF protection via Shopify.  
5. Conduct periodic passive OSINT reviews every 6–12 months.

---

## Evidence and Screenshots
All screenshots and findings are documented in the report file:  
**purelyess Passive Reconnaissance Scan Report.docx**  

Screenshots include:  
- WHOIS Lookup  
- DNS Record Enumeration  
- WAF/CDN Detection  
- SpiderFoot Passive Results  

---

## Repository Structure
