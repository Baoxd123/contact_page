# UGA CS Research Scans

This page describes a research project conducted by the **School of Computing at the University of Georgia (UGA)**. As part of this project, we perform Internet-wide **TLS/HTTPS scanning** using [`ZGrab2`](https://github.com/zmap/zgrab2) to collect publicly accessible HTML and certificate data. If you were redirected to this page from a scanning IP, this page provides details about our scanning methodology and purpose.

---

## Why am I being scanned?

You are seeing connections from us as part of an academic research project aiming to analyze **TLS certificate usage and webpage content across the Internet** to study:

- The dynamics of **SSL certificate rotation**
- Indicators of **BGP hijacking incidents**

Our system periodically performs **HTTPS/TLS handshakes** and retrieves **HTML content** from publicly reachable IP addresses and domain names. Each scan involves a **single, standard-compliant request** to port 443 (HTTPS) or 80 (HTTP), depending on the scan type.

We **do not** attempt:
- To exploit vulnerabilities
- To guess credentials or inject payloads
- To send high traffic or overload services

All scans are **non-intrusive**, **read-only**, and conform to standard protocol behavior.

---

## What data are we collecting?

We collect only:
- TLS certificates presented by servers
- Server response headers and HTML landing pages
- Timestamp, IP address, and associated domain name

This information is **already publicly accessible** to any browser connecting to your server. We do not store or analyze sensitive content or user information.

The data is used exclusively for **academic purposes**, including peer-reviewed research and conference presentations. No commercial usage is involved.

---

## IP Addresses Used for Scanning

The scans originate from the following IP addresses:

128.192.12.100 - 128.192.12.126

(Subnet: `128.192.12.100/27`)

We recommend allowlisting or blocklisting this range as appropriate to your policy. The range is **static and dedicated exclusively to research scanning.**

---

## Opt-Out

If you wish to opt out from our measurements, please email us at:

📩 **[xingda.bao@uga.edu](mailto:xingda.bao@uga.edu)**

Include the IP range or domain name you would like to exclude, and we will honor the request promptly.

---

## Contact

This scanning infrastructure is maintained by:

**Xingda Bao**  
Graduate Research Assistant 
University of Georgia, Department of Computer Science  
📧 [xingda.bao@uga.edu](mailto:xingda.bao@uga.edu)

For any concerns, abuse complaints, or collaboration inquiries, please contact us directly.

---

## About the Research

This scanning is part of a security research project focused on:
- Detecting **misissued or reverted SSL certificates** as potential indicators of BGP hijacking
- Analyzing **certificate ecosystems and trends**
- Contributing to the scientific community through open, reproducible measurements

We follow best practices for responsible Internet measurement and aim to **minimize any disruption** caused by our scans. Our research results are published in aggregated form without identifying individual IP addresses or networks.

