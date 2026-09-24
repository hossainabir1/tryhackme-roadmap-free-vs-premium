# TryHackMe Roadmap 2026: Free Rooms vs Premium Rooms (Beginner to Professional)

> A complete, step-by-step **TryHackMe learning path** that separates **free rooms** from **premium (subscription-only) rooms** at every stage — so you can go from absolute beginner to job-ready penetration tester or SOC analyst without hitting a paywall halfway through a path.

![TryHackMe](https://img.shields.io/badge/TryHackMe-Roadmap-red) ![Free Rooms](https://img.shields.io/badge/Free%20Rooms-100%2B-brightgreen) ![Level](https://img.shields.io/badge/Level-Beginner%20to%20Pro-blue) ![Updated](https://img.shields.io/badge/Updated-September%202026-lightgrey)

**Why this roadmap exists:** TryHackMe's official learning paths mix free and premium rooms together, which breaks your flow every few rooms. This guide reorders everything into a **free-first track**, lists the premium rooms separately for later, and gives a free alternative for every premium topic.

---

## Table of Contents

- [How to Use TryHackMe for Free Without Losing Momentum](#how-to-use-tryhackme-for-free-without-losing-momentum)
- [Part 1: Absolute Basics (Pre Security)](#part-1-absolute-basics-pre-security--2-weeks)
- [Part 2: Fundamentals and Tooling (Cyber Security 101 Level)](#part-2-fundamentals-and-tooling-cyber-security-101-level--3-weeks)
- [Part 3: Web Application Hacking](#part-3-web-application-hacking--4-weeks)
- [Part 4: Exploitation Tools and Your First Machines](#part-4-exploitation-tools-and-your-first-machines--4-weeks)
- [Part 5: Privilege Escalation, Active Directory and CTF Practice](#part-5-privilege-escalation-active-directory-and-ctf-practice--6-weeks)
- [Part 6: Professional Level — Specialization and Certifications](#part-6-professional-level--specialization-and-certifications)
- [Part 7: Free Alternatives for Every Premium Topic](#part-7-free-alternatives-for-every-premium-topic)
- [Part 8: Month-by-Month Study Plan and When to Buy Premium](#part-8-month-by-month-study-plan-and-when-to-buy-premium)
- [Sources](#sources)
- [Contributing](#contributing)

---

## How to Use TryHackMe for Free Without Losing Momentum

- **Skip the AttackBox, use your own Kali/Parrot VM + OpenVPN.** The free tier limits the AttackBox to 1 hour per day, but connecting your own machine over OpenVPN is unlimited and free.
- **Don't follow paths room-by-room; follow the free room order below.** Every room page shows a "Free" or "Subscription" badge, and the room search has a "Free" filter.
- **Streaks and badges count on free accounts.** Do one room or one task every day.
- **When you hit a premium room, skip it and continue.** The premium rooms are listed separately in each part so you can finish them in one month later when you subscribe.
- **Keep notes (Obsidian, Notion, or a private GitHub repo).** Write down every command and methodology — this becomes your report-writing toolkit at the professional level.

> Room free/premium status changes from time to time. Always check the badge before starting a room and open an issue in this repo if something has moved.

---

## Part 1: Absolute Basics (Pre Security) — 2 weeks

The **Pre Security path is 100% free**, so start here. Goal: understand what cyber security is, how networks and the web work, and the basic Linux and Windows commands.

### Free rooms (do in this order)

| # | Room | What you learn |
| --- | --- | --- |
| 1 | [Offensive Security Intro](https://tryhackme.com/room/offensivesecurityintro) | Your first hack — finding hidden pages on a fake bank app with Gobuster |
| 2 | [Defensive Security Intro](https://tryhackme.com/room/defensivesecurityintro) | SOC, SIEM and blue team basics |
| 3 | Careers in Cyber | Pentester vs SOC analyst vs red teamer |
| 4 | [What is Networking?](https://tryhackme.com/room/whatisnetworking) | IP, MAC, ping |
| 5 | Intro to LAN | Topologies, subnets, ARP, DHCP |
| 6 | OSI Model | The 7 layers — a permanent interview question |
| 7 | Packets & Frames | TCP handshake, ports |
| 8 | Extending Your Network | NAT, firewalls, VPN |
| 9 | [DNS in Detail](https://tryhackme.com/room/dnsindetail) | How domains resolve |
| 10 | [HTTP in Detail](https://tryhackme.com/room/httpindetail) | Requests, responses, headers, cookies |
| 11 | [How Websites Work](https://tryhackme.com/room/howwebsiteswork) | HTML/JS and your first XSS |
| 12 | [Putting it all together](https://tryhackme.com/room/puttingitalltogether) | Load balancers, CDN, WAF |
| 13 | [Linux Fundamentals Part 1](https://tryhackme.com/room/linuxfundamentalspart1) | ls, cd, cat, find, grep |
| 14 | [Linux Fundamentals Part 2](https://tryhackme.com/room/linuxfundamentalspart2) | SSH, permissions, flags |
| 15 | [Linux Fundamentals Part 3](https://tryhackme.com/room/linuxfundamentalspart3) | Cron, packages, logs |
| 16 | [Windows Fundamentals 1](https://tryhackme.com/room/windowsfundamentals1xbx) | File system, UAC, users |
| 17 | [Windows Fundamentals 2](https://tryhackme.com/room/windowsfundamentals2x0x) | msconfig, registry, task manager |
| 18 | [Windows Fundamentals 3](https://tryhackme.com/room/windowsfundamentals3xzx) | Defender, firewall, BitLocker |

### Premium rooms at this level

None — Pre Security is entirely free. Finishing the path gives you your first certificate for LinkedIn.

**Optional free extras:** [Search Skills](https://tryhackme.com/room/searchskills), Tutorial, OpenVPN (needed to connect your own VM).

---

## Part 2: Fundamentals and Tooling (Cyber Security 101 Level) — 3 weeks

This is where the first paywall appears: roughly half of the **Cyber Security 101** path is premium. Follow the free order below instead — the same topics are covered.

### Free rooms

| # | Room | Topic |
| --- | --- | --- |
| 1 | [Introductory Networking](https://tryhackme.com/room/introtonetworking) | OSI/TCP-IP recap, ping, traceroute, whois, dig |
| 2 | [Network Services](https://tryhackme.com/room/networkservices) | Enumerate and exploit SMB, Telnet, FTP |
| 3 | [Network Services 2](https://tryhackme.com/room/networkservices2) | NFS, SMTP, MySQL |
| 4 | [Nmap](https://tryhackme.com/room/furthernmap) | Full Nmap: scan types, NSE scripts |
| 5 | Nmap Live Host Discovery | ARP/ICMP host discovery |
| 6 | [Passive Reconnaissance](https://tryhackme.com/room/passiverecon) | whois, nslookup, Shodan |
| 7 | [Active Reconnaissance](https://tryhackme.com/room/activerecon) | Browser dev tools, ping, telnet |
| 8 | Traffic Analysis Essentials | What packets are and how to read them |
| 9 | [Encryption - Crypto 101](https://tryhackme.com/room/encryptioncrypto101) | RSA, SSH keys, GPG |
| 10 | [Crack the Hash](https://tryhackme.com/room/crackthehash) | Hashcat and John hands-on |
| 11 | [Hydra](https://tryhackme.com/room/hydra) | Brute-forcing SSH and web logins |
| 12 | Bash Scripting | Automation basics |
| 13 | Python Basics | Writing your own tools |
| 14 | Regular Expressions | Regex for logs and grep |

### Premium rooms (Cyber Security 101) — and their free coverage

| Premium room | Topic | Covered for free by |
| --- | --- | --- |
| Windows Command Line | cmd basics | Windows Fundamentals 1–3 + practice on your own PC |
| Windows PowerShell | PowerShell basics | Microsoft Learn PowerShell modules |
| Linux Shells | Shell scripting | Bash Scripting room |
| Networking Concepts / Essentials / Core Protocols / Secure Protocols | Modern networking module | Introductory Networking + Part 1 network rooms |
| Wireshark: The Basics | Packet analysis GUI | Traffic Analysis Essentials + Wireshark installed locally |
| Tcpdump: The Basics | CLI packet capture | Try it yourself after Wireshark |
| Nmap: The Basics | Nmap intro | The free Nmap room (more detailed) |
| Cryptography Basics / Public Key Crypto / Hashing Basics | Crypto theory | Encryption - Crypto 101 + Crack the Hash |
| John the Ripper: The Basics | Password cracking | Crack the Hash |
| Gobuster: The Basics | Directory brute force | Content Discovery (Part 3) |
| Shells Overview | Reverse/bind shells | What the Shell? (Part 4) |
| SQLMap: The Basics | Automated SQLi | SQL Injection room (Part 3) |
| CyberChef / CAPA / REMnux / FlareVM | Defensive tooling | Use CyberChef online for free |

---

## Part 3: Web Application Hacking — 4 weeks

Web hacking has the most free content on TryHackMe. You do not need the Jr Penetration Tester web module — the free rooms cover the full OWASP Top 10.

### Free rooms

| # | Room | Topic |
| --- | --- | --- |
| 1 | [Web Application Basics](https://tryhackme.com/room/webapplicationbasics) | URLs, headers, methods, status codes |
| 2 | [Walking An Application](https://tryhackme.com/room/walkinganapplication) | Manual recon with dev tools |
| 3 | Content Discovery | robots.txt, Gobuster, ffuf |
| 4 | Subdomain Enumeration | OSINT, brute force, vhosts |
| 5 | Authentication Bypass | Username enumeration, logic flaws |
| 6 | IDOR | Insecure direct object references |
| 7 | [File Inclusion](https://tryhackme.com/room/filepathtraversal) | LFI/RFI, path traversal |
| 8 | [SSRF](https://tryhackme.com/room/ssrfhr) | Server-side request forgery |
| 9 | [XSS](https://tryhackme.com/room/axss) | Reflected, stored, DOM |
| 10 | Command Injection | OS command injection |
| 11 | [SQL Injection](https://tryhackme.com/room/sqlinjectionlm) | In-band, blind, union |
| 12 | [OWASP Top 10 - 2021](https://tryhackme.com/room/owasptop102021) | All ten, hands-on |
| 13 | [Burp Suite: The Basics](https://tryhackme.com/room/burpsuitebasics) | Proxy, target, intercept |
| 14 | [Burp Suite: Repeater](https://tryhackme.com/room/burpsuiterepeater) | Modify and resend requests |
| 15 | [Introduction to OWASP ZAP](https://tryhackme.com/room/learnowaspzap) | Free Burp alternative |
| 16 | [OWASP Juice Shop](https://tryhackme.com/room/owaspjuiceshop) | OWASP practice on a real app |
| 17 | [CSRF](https://tryhackme.com/room/csrfV2) | Cross-site request forgery |
| 18 | [NoSQL Injection](https://tryhackme.com/room/nosqlinjectiontutorial) | MongoDB injection |
| 19 | [OWASP Broken Access Control](https://tryhackme.com/room/owaspbrokenaccesscontrol) | Access control bypass |
| 20 | [Advanced SQL Injection](https://tryhackme.com/room/advancedsqlinjection) | Second-order, out-of-band |
| 21 | [DVWA](https://tryhackme.com/room/dvwa) / [WebGOAT](https://tryhackme.com/room/webgoat) | Practice playgrounds |

**Free web CTFs:** [Overpass](https://tryhackme.com/room/overpass), [Bolt](https://tryhackme.com/room/bolt), Takeover, Corridor, [Pickle Rick](https://tryhackme.com/room/picklerick), [RootMe](https://tryhackme.com/room/rrootme).

### Premium rooms (Jr Penetration Tester web module) — and their free coverage

| Premium room | Topic | Covered for free by |
| --- | --- | --- |
| Burp Suite: Intruder / Other Modules / Extensions | Advanced Burp | PortSwigger Web Security Academy Burp labs |
| Web Enumeration / Web Recon module | Structured recon | Content Discovery + Subdomain Enumeration |
| Race Conditions | Web race conditions | PortSwigger Academy race condition labs |
| XXE Injection | XML external entities | PortSwigger Academy XXE labs |
| Insecure Deserialization | Object injection | PortSwigger Academy deserialization labs |
| API Testing / Broken Authentication (2025 module) | API security | PortSwigger API labs + OWASP crAPI |
| Web Application Pentesting capstones | End-to-end challenge | Free CTF list above |

> **PortSwigger Web Security Academy** (portswigger.net/web-security) is completely free and goes deeper than TryHackMe premium on web — skipping the premium web rooms costs you nothing.

---

## Part 4: Exploitation Tools and Your First Machines — 4 weeks

Here you run the full chain for the first time: **scan → enumerate → exploit → shell**. The core rooms of the Jr Penetration Tester "Vulnerability Research" and "Metasploit" modules are free.

### Free rooms

| # | Room | Topic |
| --- | --- | --- |
| 1 | [Vulnerabilities 101](https://tryhackme.com/room/vulnerabilities101) | CVE, CVSS, NVD, Exploit-DB |
| 2 | Exploit Vulnerabilities | Searchsploit, manual exploitation |
| 3 | [Metasploit: Introduction](https://tryhackme.com/room/metasploitintro) | msfconsole, modules |
| 4 | Metasploit: Exploitation | Scan + exploit + msfvenom |
| 5 | Metasploit: Meterpreter | Post-exploitation shell |
| 6 | [What the Shell?](https://tryhackme.com/room/introtoshells) | Reverse/bind shells, netcat, shell stabilisation |
| 7 | Protocols and Servers 1 & 2 | Attacking FTP/SMTP/POP3/IMAP and their secure versions |
| 8 | [Hydra](https://tryhackme.com/room/hydra) (recap) | Brute-force logins |
| 9 | Common Linux Privesc | First taste of privilege escalation |

### Your first 8 machines (free, in this order)

| # | Room | Why |
| --- | --- | --- |
| 1 | [Vulnversity](https://tryhackme.com/room/vulnversity) | Nmap + Gobuster + upload bypass + privesc — the full chain |
| 2 | [Blue](https://tryhackme.com/room/blue) | Windows via EternalBlue with Metasploit |
| 3 | [Simple CTF](https://tryhackme.com/room/easyctf) | Find a CVE and exploit it |
| 4 | [Bounty Hacker](https://tryhackme.com/room/cowboyhacker) | Anonymous FTP + Hydra + sudo privesc |
| 5 | Brute It | Hydra + John + privesc |
| 6 | [Kenobi](https://tryhackme.com/room/kenobi) | Samba + ProFTPD + SUID |
| 7 | [RootMe](https://tryhackme.com/room/rrootme) | Upload bypass + SUID python |
| 8 | Agent Sudo / Lazy Admin | Steganography + CMS exploitation |

### Premium rooms (Jr Penetration Tester) — and their free coverage

| Premium room | Topic | Covered for free by |
| --- | --- | --- |
| Pentesting Fundamentals / Principles of Security | Methodology, rules of engagement | Careers in Cyber + OWASP Testing Guide (free PDF) |
| Passive/Active Recon (2026 rebuilt versions) | Recon | The older free Passive/Active Reconnaissance rooms |
| Net Sec Challenge | Nmap challenge box | Nmap room + Vulnversity |
| Shells Overview / Enumeration & Brute Force | Shells + enumeration | What the Shell? |
| Metasploit: Post Exploitation (new) | Persistence, pivoting | Meterpreter room + Metasploit docs |
| Jr Pentester capstone challenges (3 new in 2026) | End-to-end | Free machine list above |

---

## Part 5: Privilege Escalation, Active Directory and CTF Practice — 6 weeks

You are now intermediate. The core privesc and AD rooms are free — spend the most time here, because this is what both PT1 and OSCP test.

### Free rooms — Privilege Escalation

| # | Room | Topic |
| --- | --- | --- |
| 1 | [Linux Privilege Escalation](https://tryhackme.com/room/linprivesc) | Kernel, sudo, SUID, cron, PATH, NFS — everything |
| 2 | [Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | Older version, extra practice |
| 3 | [Linux PrivEsc Arena](https://tryhackme.com/room/linuxprivescarena) | 20+ privesc exercises |
| 4 | [Windows PrivEsc](https://tryhackme.com/room/windows10privesc) | Services, registry, tokens, DLL hijacking |
| 5 | [Windows PrivEsc Arena](https://tryhackme.com/room/windowsprivescarena) | Windows practice |
| 6 | [Sudo Security Bypass](https://tryhackme.com/room/sudovulnsbypass) / [Sudo Buffer Overflow](https://tryhackme.com/room/sudovulnsbof) | CVE-based privesc |
| 7 | [Linux Agency](https://tryhackme.com/room/linuxagency) | 30+ level Linux privesc marathon |

### Free rooms — Active Directory

| # | Room | Topic |
| --- | --- | --- |
| 1 | [Active Directory Basics](https://tryhackme.com/room/winadbasics) | Domains, OUs, GPOs, Kerberos |
| 2 | [Breaching Active Directory](https://tryhackme.com/room/breachingad) | NTLM, LDAP, password spraying |
| 3 | [Attacktive Directory](https://tryhackme.com/room/attacktivedirectory) | Kerbrute + AS-REP roasting + secretsdump |
| 4 | [Post-Exploitation Basics](https://tryhackme.com/room/postexploit) | BloodHound, Mimikatz |
| 5 | [Enterprise](https://tryhackme.com/room/enterprise) / [RazorBlack](https://tryhackme.com/room/raz0rblack) | Medium AD boxes |
| 6 | [Active Directory Hardening](https://tryhackme.com/room/activedirectoryening) | The defensive side |

### Free CTF grind (one per day)

- **Easy:** [Blaster](https://tryhackme.com/room/blaster), Ignite, Startup, Lian Yu, Break Out The Cage, B3dr0ck, Anthem, Blueprint, Retro
- **Medium:** [Mr Robot CTF](https://tryhackme.com/room/mrrobot), [GoldenEye](https://tryhackme.com/room/goldeneye), [Wonderland](https://tryhackme.com/room/wonderland), [Relevant](https://tryhackme.com/room/relevant), Dogcat, VulnNet: Active, Ollie, Eavesdropper
- **Buffer overflow (OSCP-style):** [Buffer Overflow Prep](https://tryhackme.com/room/bufferoverflowprep), [Gatekeeper](https://tryhackme.com/room/gatekeeper), [Intro To Pwntools](https://tryhackme.com/room/introtopwntools)

### Premium rooms at this level — and their free coverage

| Premium room | Topic | Covered for free by |
| --- | --- | --- |
| Intro to AD Breaching / Authenticated Enumeration / Credential Harvesting / Lateral Movement (2026 Jr Pentester AD module) | Structured AD attack chain | Breaching AD + Post-Exploitation Basics + Attacktive Directory |
| Active Directory Challenge 1 (new) | AD capstone | Enterprise, RazorBlack |
| Enumerating / Lateral Movement & Pivoting / Exploiting / Persisting AD (Red Team path) | Deep AD | Free AD list above + HackTheBox free AD boxes |
| Wreath | Network pivoting | No free equivalent — the single most valuable premium room; do it first when you subscribe |
| Holo | AD network simulation | After Wreath |
| Throwback | AD network | After Holo |

---

## Part 6: Professional Level — Specialization and Certifications

After Part 5 you are entry-level job ready. Pick a lane: **Red team (pentesting)** or **Blue team (SOC)**. Both exist on TryHackMe, but the paths at this level are mostly premium — this is where a one-month subscription pays for itself.

### Red team lane

| Path | Free / Premium | Notes |
| --- | --- | --- |
| Jr Penetration Tester (89 rooms, 17 modules, ~70–90 hours) | Mixed, ~40% free | Parts 3–5 already cover half of it; the premium half takes about a month |
| Offensive Pentesting | Mostly premium | Free: [Kenobi](https://tryhackme.com/room/kenobi), [Blue](https://tryhackme.com/room/blue), [Relevant](https://tryhackme.com/room/relevant), Buffer Overflow Prep, Attacktive Directory, Gatekeeper |
| Red Teaming | Mostly premium | Free: [Red Team Recon](https://tryhackme.com/room/redteamrecon), [Red Team OPSEC](https://tryhackme.com/room/opsec), Red Team Fundamentals, Intro to Antivirus |

### Blue team lane

| Path | Free / Premium | Notes |
| --- | --- | --- |
| SOC Level 1 | Mixed | Free: Snort, Traffic Analysis Essentials, Windows Forensics 1, Linux Process Analysis, Phishing Analysis, Threat Hunting: Foothold + 40 free forensics rooms |
| SOC Level 2 | Premium | Prep for SAL2 |
| Cyber Defense | Mixed | Free forensics/log-analysis rooms cover most of it |

### Certification order

| Cert | For | Format | Price (USD) | Prerequisite |
| --- | --- | --- | --- | --- |
| SEC0 (Pre-Security) | Complete beginners | Practical tasks | Low; 20% off bundled with SEC1 | Part 1 |
| SEC1 (Security 101) | Foundation proof | Practical assessment | 15% off with Premium | Part 2 |
| PT1 (Junior Penetration Tester) | Red team entry | 48-hour practical + graded report | $297 (includes 3 months Premium + 1 retake) | Parts 3–5 + Jr Pentester path |
| SAL1 (Security Analyst Level 1) | SOC entry | Live SOC simulator + incident report | $349 (includes 3 months Premium + 1 retake) | SOC Level 1 path |
| SAL2 | Mid-level SOC | Multi-stage investigations | 15% off with Premium | SAL1 |
| AI1 (AI Security) | Specialist | 13 hands-on scenarios | 15% off with Premium | PT1 or SAL1 |

PT1 and SAL1 are valid for 3 years; the exam attempt must be used within 12 months of purchase. **Most cost-effective route:** buying PT1 ($297) includes 3 months of Premium, so buy the cert instead of a standalone subscription and get all premium rooms plus the exam together.

### Certifications outside TryHackMe

| Cert | Price | When |
| --- | --- | --- |
| eJPT (INE) | ~$250 | PT1 alternative, better known to HR |
| CompTIA Security+ | ~$400 | Passing HR filters for blue team jobs |
| OSCP (OffSec) | ~$1,750 | 1–2 years in, after Part 5 buffer overflow + AD |
| CPTS (HackTheBox) | ~$210 | Cheaper and harder OSCP alternative |

> Prices are as of September 2026 — verify on the official sites before buying.

---

## Part 7: Free Alternatives for Every Premium Topic

| Premium topic | Free alternative | Link |
| --- | --- | --- |
| Advanced Burp, XXE, deserialization, race conditions, API | PortSwigger Web Security Academy — 200+ labs | portswigger.net/web-security |
| Wireshark / Tcpdump | Install Wireshark and work through pcap exercises | malware-traffic-analysis.net |
| Wreath / Holo / Throwback (pivoting, AD networks) | HackTheBox free retired machines + HTB Academy free tier; build GOAD (Game of AD) locally | hackthebox.com, github.com/Orange-Cyberdefense/GOAD |
| Windows CLI / PowerShell | Microsoft Learn PowerShell modules | learn.microsoft.com/powershell |
| Red Team path (C2, evasion) | TCM Security free YouTube courses, MalDev Academy free section | youtube.com/@TCMSecurityAcademy |
| SOC Level 1 premium (SIEM, Splunk) | Splunk Boss of the SOC datasets, LetsDefend free tier, CyberDefenders free challenges | letsdefend.io, cyberdefenders.org |
| Metasploit post-exploitation | OffSec Metasploit Unleashed | offsec.com/metasploit-unleashed |
| OSCP-style practice boxes | VulnHub (free offline VMs) | vulnhub.com |

**Rule:** if you get stuck on one platform, do the same topic on another — but keep the TryHackMe free list as your main track, or everything ends up half-finished.

---

## Part 8: Month-by-Month Study Plan and When to Buy Premium

At 1.5–2 hours per day, Parts 1–5 take about 6 months on the free tier; you are PT1-ready around month 7–8.

| Month | What to do | Free / Premium |
| --- | --- | --- |
| 1 | All of Part 1 (Pre Security) + Kali VM + OpenVPN setup + note system | Free |
| 2 | Part 2 free rooms + Bash/Python basics | Free |
| 3 | Part 3 web rooms 1–16 + PortSwigger SQLi/XSS labs | Free |
| 4 | Rest of Part 3 + Part 4 tools + first 8 machines | Free |
| 5 | Part 5 privesc (Linux + Windows) + one easy CTF per day | Free |
| 6 | Part 5 AD + medium CTFs + buffer overflow | Free |
| 7 | **Buy PT1 / Premium** — Jr Pentester premium rooms + Wreath + Holo + capstones | Premium (3 months included with PT1) |
| 8 | PT1 exam + report practice; or SOC Level 1 premium rooms for the blue lane | Premium |
| 9+ | Red Teaming path / SOC Level 2, HackTheBox, eJPT or OSCP prep | Mixed |

### Should you buy Premium?

- **Not yet.** Parts 1–5 contain 100+ free rooms — about 6 months of work. Buying now means paying for months where you would not open a premium room.
- **In month 7, buy the PT1 exam ($297) instead of a subscription.** It includes 3 months of Premium; 3 months at $16.99 would cost $51 on its own.
- If you only need the subscription, the **annual student plan** (~$8.33/month, .edu email required) is the cheapest option.
- Once on Premium, do these first: Wreath → Jr Pentester AD module → Holo → Throwback → capstones. None have free equivalents and they are the most job-relevant.

### Daily routine

- [ ] One room or one CTF (keep the streak)
- [ ] Add commands and methodology to your notes
- [ ] Once a week: re-solve an old CTF without notes (retention check)
- [ ] Once a month: re-check room badges in this list for free/premium changes

---

## Sources

- [TryHackMe — Free TryHackMe Training: The Ultimate Guide for Beginners](https://tryhackme.com/resources/blog/free_path)
- [TryHackMe — Free Rooms](https://tryhackme.com/free-rooms)
- [TryHackMe — Jr Penetration Tester Learning Path Rebuilt for 2026](https://tryhackme.com/resources/blog/jr-penetration-tester-learning-path-rebuilt-for-2026)
- [TryHackMe — Certification Guide 2026](https://tryhackme.com/resources/blog/tryhackme-certification-guide)
- [HackerDNA — TryHackMe Certifications 2026: SAL1 & PT1 Cost + Validity](https://hackerdna.com/blog/tryhackme-certifications)
- [CertCompass — TryHackMe Review 2026](https://certcompass.org/tryhackme-review-2026/)
- [winterrdog/tryhackme-free-rooms](https://github.com/winterrdog/tryhackme-free-rooms)
- [Hunterdii/TryHackMe-Roadmap](https://github.com/Hunterdii/TryHackMe-Roadmap)

## Contributing

Found a room that moved from free to premium (or the other way)? Open an issue or a pull request with the room link and the date you checked. Stars help other beginners find this roadmap.

**Keywords:** TryHackMe roadmap, TryHackMe free rooms, TryHackMe premium rooms list, TryHackMe learning path 2026, cybersecurity roadmap for beginners, how to learn ethical hacking for free, PT1 certification study plan, SAL1 study plan, Jr Penetration Tester path free rooms, OSCP preparation TryHackMe.

## License

MIT — free to fork, translate and share with attribution.
