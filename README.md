# PurelyEss-Passive-Reconnaissance
Passive reconnaissance and OSINT analysis of PurelyEss.com — identifying domain, DNS, and CDN security posture using ethical open-source intelligence methods.
# 🕵️ Passive Reconnaissance & OSINT Report – PurelyEss.com

### Author
**Emmanuel Oladeinde**  
Cybersecurity Analyst | Defensive & Reconnaissance Specialist

---

## 📄 Project Overview
This repository contains a **passive reconnaissance assessment** of the domain **PurelyEss.com**, performed in **November 2025**.  
The purpose of this project was to identify publicly available intelligence about the target domain using **ethical OSINT techniques** only — no intrusive or exploitative activity was conducted.

---

## 🎯 Objectives
- Map the domain’s public exposure surface.
- Identify registrar, DNS, and WAF/CDN details.
- Assess the presence of DNSSEC, SPF, DKIM, DMARC, and HTTP security headers.
- Discover any public leaks or exposures using passive OSINT tools.

---

## 🧰 Tools & Frameworks Used
| Category | Tool / Source | Purpose |
|-----------|---------------|----------|
| Domain & WHOIS | `whois`, `rdap` | Registration and expiration details |
| DNS Enumeration | `dig`, `dnsrecon` | Identify A/AAAA, NS, MX, TXT, CAA records |
| WAF Detection | `wafw00f` | Identify CDN/WAF infrastructure |
| OSINT Automation | `SpiderFoot (passive modules)` | Subdomain and credential discovery |
| Banner & Header Review | `Wapiti` | Web header fingerprinting |
| OSINT References | `OSINT Framework` | Public CT logs, paste sites, reputation databases |

---

## 🧩 Key Findings (Summary)
- The domain is **hosted on Shopify CDN** (`23.227.38.32`), providing built-in WAF and DDoS mitigation.  
- **DNSSEC** not enabled.  
- Missing security headers (**HSTS, CSP, Referrer-Policy**).  
- No exposed credentials or sensitive data detected in passive OSINT sources.  

**Overall Exposure Rating:** `Low to Moderate`

---

## 🛡️ Recommendations
1. **Enable DNSSEC** at registrar level (GoDaddy).  
2. **Implement security headers** (HSTS, CSP, Referrer-Policy, Permissions-Policy).  
3. **Deploy SPF, DKIM, DMARC** for mail authentication.  
4. **Maintain CDN/WAF coverage** via Shopify for continuous protection.  
5. **Perform passive OSINT reviews** every 6–12 months to detect new subdomains or leaks.

---

## 📸 Evidence & Screenshots
All relevant screenshots and findings are documented inside the project’s report file:  
**`purelyess Passive Reconnaissance Scan Report.docx`**  
Each section includes visuals for:
- WHOIS Lookup  
- DNS Record Discovery  
- WAF/CDN Fingerprint  
- SpiderFoot Passive Scan Results  

---

## 📁 Repository Structure
