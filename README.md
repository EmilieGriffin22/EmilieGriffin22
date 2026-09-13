# Emilie Griffin

Security and Systems Engineering · M.S. Computer Science, University at Buffalo, May 2027
Currently: AI Solutions Intern at Ingersoll Rand
 
I do my best work in the layer where software meets the network — building protocols from raw sockets, finding the places where access control doesn't quite hold, and writing the tools that catch it next time.
 
**Splunk Core Certified Power User** · Teaching Assistant, Systems Programming · 1st place, UB Network Defense Club Red vs. Blue (internal division)
 
---
 
## What I've Built
 
My strongest work isn't in this profile, and for good reason. My master's capstone is a live client's administrative codebase. My automated testing suites and document ingestion process are actively used in enterprise settings. The protocol implementations are coursework for classes my own department still assigns. And I TA in that department. So instead of dumping code I can't publish, here's what the work actually was:
 
### Vulnerability assessment and hardening — master's capstone, live client
Assessed a production Django backend and patched 12 real vulnerabilities: unauthenticated endpoints, missing rate limiting, and a complete lack of access-control separation between employee groups. Built token-based auth compatible with the client's iOS app, a 50+ permission RBAC framework, and rate limiting across every endpoint.

Midway through, the client was hit by a live DoS attack — and messaged me immediately. After pulling her server logs into a Grafana dashboard to make the traffic legible, I found hundreds of fraudulent account registrations and thousands of spam requests originating from a single foreign IP range with no legitimate users behind it. As such, we blocked the range to stop the bleeding while the rate limiting I'd already designed finished its way to production. Blocking IPs isn't a fix. But it bought the days we needed for the real one.

### Automated access-control verification — Regeneron, IT Applications (2025)
Built a 100+ test Cypress suite across more than 50 endpoints to verify (continuously) that access control actually held at every permission level of a live .NET application. This work surfaced a privilege escalation issue that let unauthorized users reach sensitive information, something I worked with the development team to patch and document before the release shipped.

### Document processing at enterprise scale — M&T Bank 
Designed a reusable .NET application automating document ingestion into an enterprise CMS across four home-ownership applications: REST APIs, SQL Server, Automic for scheduling, validation logic, and status-dependent routing with logging that makes the pipeline auditable. Supports 15,000+ transactions annually and eliminated 2,000+ hours of manual processing.

### Threat intelligence — Regeneron, Information Security (2024)
Profiled 300+ phishing domains impersonating company brands, and mapped the infrastructure (DNS registration patterns, IP clustering, hosting) into a MITRE ATT&CK-mapped threat model and actor profile. Ingested hundreds of IOCs into Splunk for correlation. Ran SafeBreach attack simulations whose findings scoped the next quarter's phishing awareness campaign.
 
### HTTP/1.1 and WebSocket, from raw TCP sockets
Wrote the server by hand in Python: request-line and CRLF header parsing, cookies, multipart bodies, GET/POST/PATCH/DELETE. Then TLS, OAuth 2.0 against GitHub, upload handling, and slow-send DoS timeout mitigation. Implemented RFC 6455 from the spec — handshake upgrade, frame parsing, FIN bit, opcode, masking — to carry a collaborative drawing board and a multi-user video room.
 
### Kademlia DHT and Raft consensus, in Go
Full node lifecycle, routing table management, and iterative FIND_NODE with fault-tolerant peer discovery over TCP with Protocol Buffers. Raft with leader election, log replication, the full follower/candidate/leader state machine, and heartbeat failure detection.

### Multi-agent LLM pipeline — TechBuffalo Design Challenge with 43North  
Led a 3-agent pipeline (Anthropic Claude, Google Gemini) that ingests prospecting email, extracts structured startup profiles, and matches them against a partner network. Built two-tier model routing with prompt caching and token budgets so the whole thing could be tested end to end for free.
 
---
 
## Stack

**Languages** C#, Python, Go, C, Java, SQL, Bash  
**Security** Splunk, Wireshark, tcpdump, Snort, Nmap, Metasploit, Anomali ThreatStream, MITRE ATT&CK, Grafana  
**Frameworks & Tools** .NET / ASP.NET, Django, Flask, REST APIs, Cypress, Automic  
**Platforms** Linux, Windows, Docker, Git, Active Directory  
 
---
 
📍 Buffalo, NY · [LinkedIn](https://linkedin.com/in/emilie-griffin) · emiliegriffin04@gmail.com
