# Hands-on-Nmap-Reconnaissance-NSE-Scripting-Firewall-Evasion-Wireshark-Packet-Analysis-CTF-Labs-
A practical collection of cybersecurity CTF labs covering advanced network discovery (Nmap fundamentals, host discovery, port scanning, service enumeration, OS fingerprinting, vulnerability scanning), custom NSE scripting &amp; firewall/IDS evasion, and deep packet traffic analysis (HTTP headers, TLS handshakes, malware beacons, advanced PCAP relays).
# Nmap Reconnaissance, NSE Scripting, Firewall Evasion & Deep Packet Analysis CTF Labs

Welcome to the **Nmap Reconnaissance, NSE Scripting, Firewall Evasion & Deep Packet Analysis CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on network-level host discovery, service enumeration, evasion craft, and protocol-level packet analysis—spanning **Nmap Reconnaissance & Network Fingerprinting (Host discovery, port scanning, service enumeration, OS detection, vulnerability validation)**, **Custom Automation & Evasion Tradecraft (NSE Lua scripting, firewall/IDS evasion techniques)**, and **Deep Packet Inspection & Network Forensics (HTTP header analysis, TLS SNI/handshake dissection, C2 malware beacon hunting, silent relay packet analysis)**.

---

## Lab Collection Index

### 1. Nmap Reconnaissance, Service Fingerprinting & Vulnerability Scanning
* **Nmap Fundamentals: From Discovery to Service Mapping**  
  *Lab Link:* [https://learn.secbyte.org/ctf/nmap-fundamentals-from-discovery-to-service-mapping](https://learn.secbyte.org/ctf/nmap-fundamentals-from-discovery-to-service-mapping)  
  *Focus:* Core principles of Nmap execution, target specification syntaxes, service version probing (`-sV`), default script execution (`-sC`), and output formatting (`-oA`).

* **Host Discovery: Finding the Hidden Fleet**  
  *Lab Link:* [https://learn.secbyte.org/ctf/host-discovery-finding-the-hidden-fleet](https://learn.secbyte.org/ctf/host-discovery-finding-the-hidden-fleet)  
  *Focus:* Discovering live hosts across non-responsive subnets using ARP ping (`-PR`), ICMP echo/timestamp requests (`-PE`/`-PP`), TCP SYN/ACK ping probes (`-PS`/`-PA`), and UDP ping (`-PU`).

* **Port Scanning: Recon in the Dark**  
  *Lab Link:* [https://learn.secbyte.org/ctf/port-scanning-recon-in-the-dark](https://learn.secbyte.org/ctf/port-scanning-recon-in-the-dark)  
  *Focus:* Executing stealthy TCP SYN scans (`-sS`), full TCP connect scans (`-sT`), UDP port scans (`-sU`), and specialized scan types (FIN `-sF`, NULL `-sN`, Xmas `-sX`).

<Image src="image_agent_tag_13074652173350385338" alt="Nmap port scanning risks and operational warnings diagram" caption="Nmap Network Scanning Operations & Risk Considerations" />

---

* **Service Enumeration: The Forgotten Estate**  
  *Lab Link:* [https://learn.secbyte.org/ctf/service-enumeration-the-forgotten-estate](https://learn.secbyte.org/ctf/service-enumeration-the-forgotten-estate)  
  *Focus:* Probing unmapped high-range ports (`-p-`), banner grabbing legacy service daemons, evaluating protocol response signatures, and cataloging enterprise shadow IT assets.

* **OS Detection: From Fingerprints to Forensic Confidence**  
  *Lab Link:* [https://learn.secbyte.org/ctf/os-detection-from-fingerprints-to-forensic-confidence](https://learn.secbyte.org/ctf/os-detection-from-fingerprints-to-forensic-confidence)  
  *Focus:* Analyzing remote OS fingerprinting mechanics (`-O`), evaluating TCP/IP stack implementation variations (window sizes, TTL defaults, TCP options), and interpreting match confidence percentages.

* **Vulnerability Scanning Fundamentals: From Discovery to Validation**  
  *Lab Link:* [https://learn.secbyte.org/ctf/vulnerability-scanning-fundamentals-from-discovery-to-valida](https://learn.secbyte.org/ctf/vulnerability-scanning-fundamentals-from-discovery-to-valida)  
  *Focus:* Leveraging Nmap vulnerability databases (`vuln` script category), validating CVE exposures, distinguishing false positives from confirmed vulnerabilities, and scoring severity metrics.

### 2. NSE Scripting & Firewall/IDS Evasion Tradecraft
* **NSE Scripting: From Discovery to Custom Automation**  
  *Lab Link:* [https://learn.secbyte.org/ctf/nse-scripting-from-discovery-to-custom-automation](https://learn.secbyte.org/ctf/nse-scripting-from-discovery-to-custom-automation)  
  *Focus:* Authoring custom Lua-based Nmap Scripting Engine (NSE) scripts, defining rule triggers (`portrule`, `hostrule`), parsing socket responses, and automating specialized scanning tasks.

* **Firewall Evasion Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/firewall-evasion-lab](https://learn.secbyte.org/ctf/firewall-evasion-lab)  
  *Focus:* Bypassing stateful firewalls and intrusion detection systems (IDS)—utilizing IP fragmentation (`-f`), MTU sizing (`--mtu`), decoy IP addresses (`-D`), source port spoofing (`--source-port`), and MAC address spoofing.

### 3. Deep Packet Inspection & Network Traffic Forensics
* **HTTP Traffic Analysis: From Headers to Hidden Sessions**  
  *Lab Link:* [https://learn.secbyte.org/ctf/http-traffic-analysis-from-headers-to-hidden-sessions](https://learn.secbyte.org/ctf/http-traffic-analysis-from-headers-to-hidden-sessions)  
  *Focus:* Inspecting unencrypted HTTP packet streams in Wireshark, reconstructing TCP streams, extracting session cookies and POST credentials, and analyzing user-agent anomalies.

<Image src="image_agent_tag_13074652173350384215" alt="Wireshark network packet analysis interface workflow diagram" caption="Wireshark Network Packet Analysis Overview" />

---

* **TLS Traffic Analysis: From Handshake to Hidden Signals**  
  *Lab Link:* [https://learn.secbyte.org/ctf/tls-traffic-analysis-from-handshake-to-hidden-signals](https://learn.secbyte.org/ctf/tls-traffic-analysis-from-handshake-to-hidden-signals)  
  *Focus:* Analyzing encrypted TLS/SSL packet captures, inspecting Client Hello Server Name Indication (SNI) extension fields, auditing X.509 certificate chains, and identifying Ja3/Ja3s fingerprint signatures.

* **Malware Traffic Analysis: Beacon Hunt**  
  *Lab Link:* [https://learn.secbyte.org/ctf/malware-traffic-analysis-beacon-hunt](https://learn.secbyte.org/ctf/malware-traffic-analysis-beacon-hunt)  
  *Focus:* Detecting periodic command-and-control (C2) beaconing patterns in PCAP data, identifying jitter calculations, isolating infected internal endpoints, and extracting malicious payload URLs.

* **Advanced Packet Investigation: Silent Relay**  
  *Lab Link:* [https://learn.secbyte.org/ctf/advanced-packet-investigation-silent-relay](https://learn.secbyte.org/ctf/advanced-packet-investigation-silent-relay)  
  *Focus:* Triaging low-level packet anomalies, detecting unauthorized DNS/ICMP tunneling exfiltration, analyzing port redirection streams, and uncovering hidden proxy relays.

---

## Learning Path

### Path A: Network Reconnaissance & Fingerprinting Specialist
1. **Scanning Fundamentals & Host Discovery:** Start with [Nmap Fundamentals](https://learn.secbyte.org/ctf/nmap-fundamentals-from-discovery-to-service-mapping), [Host Discovery](https://learn.secbyte.org/ctf/host-discovery-finding-the-hidden-fleet), and [Port Scanning](https://learn.secbyte.org/ctf/port-scanning-recon-in-the-dark).
2. **Fingerprinting & Vuln Audit:** Master asset audits via [Service Enumeration](https://learn.secbyte.org/ctf/service-enumeration-the-forgotten-estate), [OS Detection](https://learn.secbyte.org/ctf/os-detection-from-fingerprints-to-forensic-confidence), and [Vulnerability Scanning Fundamentals](https://learn.secbyte.org/ctf/vulnerability-scanning-fundamentals-from-discovery-to-valida).

### Path B: NSE Scripting & Evasion Specialist
1. **Custom Automation:** Write custom scanning routines in [NSE Scripting: From Discovery to Custom Automation](https://learn.secbyte.org/ctf/nse-scripting-from-discovery-to-custom-automation).
2. **Firewall & IDS Evasion:** Bypass perimeter controls in [Firewall Evasion Lab](https://learn.secbyte.org/ctf/firewall-evasion-lab).

### Path C: Network Forensic Examiner & Packet Analyst
1. **Cleartext & TLS Analysis:** Analyze PCAPs using [HTTP Traffic Analysis](https://learn.secbyte.org/ctf/http-traffic-analysis-from-headers-to-hidden-sessions) and [TLS Traffic Analysis](https://learn.secbyte.org/ctf/tls-traffic-analysis-from-handshake-to-hidden-signals).
2. **Malware Beacons & Tunneling:** Detect malicious streams via [Malware Traffic Analysis: Beacon Hunt](https://learn.secbyte.org/ctf/malware-traffic-analysis-beacon-hunt) and [Advanced Packet Investigation](https://learn.secbyte.org/ctf/advanced-packet-investigation-silent-relay).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, target IP specifications, Wireshark PCAP files (`.pcap`/`.pcapng`), or Lua script templates.
4. Execute tailored Nmap scans (`-sS`, `-sV`, `-O`), write custom NSE detection logic, configure IP fragmentation flags to bypass firewalls, or filter PCAPs in Wireshark (`http.request`, `tls.handshake.extensions_server_name`) to capture flags.

---

## Target Audience

* **Penetration Testers & Network Security Auditors:** Perform deep host discovery, service versioning, OS fingerprinting, custom NSE script development, and firewall evasion.
* **SOC Analysts & Network Forensics Investigators:** Inspect Wireshark packet captures, trace HTTP/TLS session flows, detect C2 malware beacons, and uncover DNS/ICMP data exfiltration.
* **Network & Systems Administrators:** Identify unauthorized shadow IT devices, audit exposed network port surfaces, and validate firewall policy enforcement.
* **Cybersecurity Students:** Acquire practical hands-on experience in Nmap command-line syntaxes, network protocol mechanics, and Wireshark PCAP analysis.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized port scanning, evasion testing, or packet interception against external production networks without explicit permission is strictly prohibited.
