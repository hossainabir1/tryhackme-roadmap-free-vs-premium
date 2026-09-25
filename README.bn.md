# ট্রাইহ্যাকমি রোডম্যাপ ২০২৬: ফ্রি রুম বনাম প্রিমিয়াম রুম (বিগিনার থেকে প্রফেশনাল)

> একটি সম্পূর্ণ, ধাপে ধাপে **TryHackMe লার্নিং পাথ** যেখানে প্রতিটি স্টেজে **ফ্রি রুম** আর **প্রিমিয়াম (সাবস্ক্রিপশন-অনলি) রুম** আলাদা করে দেওয়া আছে — যাতে তুমি একদম বিগিনার থেকে জব-রেডি পেনিট্রেশন টেস্টার বা SOC অ্যানালিস্ট পর্যন্ত পৌঁছাতে পারো, মাঝপথে পেওয়ালে আটকে না গিয়ে।

![TryHackMe](https://img.shields.io/badge/TryHackMe-Roadmap-red) ![Free Rooms](https://img.shields.io/badge/Free%20Rooms-100%2B-brightgreen) ![Level](https://img.shields.io/badge/Level-Beginner%20to%20Pro-blue) ![Updated](https://img.shields.io/badge/Updated-September%202026-lightgrey)

**এই রোডম্যাপ কেন বানানো হয়েছে:** TryHackMe-এর অফিসিয়াল লার্নিং পাথগুলোতে ফ্রি আর প্রিমিয়াম রুম মিশিয়ে রাখা হয়, ফলে কিছু রুম করার পরই ফ্লো ভেঙে যায়। এই গাইডে সব কিছু **ফ্রি-ফার্স্ট অর্ডারে** সাজানো হয়েছে, প্রিমিয়াম রুমগুলো আলাদাভাবে পরে করার জন্য লিস্ট করা আছে, আর প্রতিটি প্রিমিয়াম টপিকের জন্য একটা ফ্রি অলটারনেটিভ দেওয়া আছে।

> এই ফাইলটি মূল ইংরেজি [README.md](README.md)-এর বাংলা অনুবাদ। রুম আপডেট হলে আগে ইংরেজি ভার্সন আপডেট করে তারপর এখানে সিঙ্ক করা হবে।

---

## সূচিপত্র

- [ফ্লো না ভেঙে TryHackMe ফ্রি-তে যেভাবে ব্যবহার করবে](#ফ্লো-না-ভেঙে-tryhackme-ফ্রি-তে-যেভাবে-ব্যবহার-করবে)
- [পার্ট ১: একদম বেসিক (Pre Security)](#পার্ট-১-একদম-বেসিক-pre-security--২-সপ্তাহ)
- [পার্ট ২: ফান্ডামেন্টালস আর টুলিং (Cyber Security 101 লেভেল)](#পার্ট-২-ফান্ডামেন্টালস-আর-টুলিং-cyber-security-101-লেভেল--৩-সপ্তাহ)
- [পার্ট ৩: ওয়েব অ্যাপ্লিকেশন হ্যাকিং](#পার্ট-৩-ওয়েব-অ্যাপ্লিকেশন-হ্যাকিং--৪-সপ্তাহ)
- [পার্ট ৪: এক্সপ্লয়টেশন টুলস আর প্রথম মেশিনগুলো](#পার্ট-৪-এক্সপ্লয়টেশন-টুলস-আর-প্রথম-মেশিনগুলো--৪-সপ্তাহ)
- [পার্ট ৫: প্রিভিলেজ এস্কেলেশন, অ্যাক্টিভ ডিরেক্টরি আর CTF প্র্যাকটিস](#পার্ট-৫-প্রিভিলেজ-এস্কেলেশন-অ্যাক্টিভ-ডিরেক্টরি-আর-ctf-প্র্যাকটিস--৬-সপ্তাহ)
- [পার্ট ৬: প্রফেশনাল লেভেল — স্পেশালাইজেশন আর সার্টিফিকেশন](#পার্ট-৬-প্রফেশনাল-লেভেল--স্পেশালাইজেশন-আর-সার্টিফিকেশন)
- [পার্ট ৭: প্রতিটি প্রিমিয়াম টপিকের ফ্রি অলটারনেটিভ](#পার্ট-৭-প্রতিটি-প্রিমিয়াম-টপিকের-ফ্রি-অলটারনেটিভ)
- [পার্ট ৮: মাস অনুযায়ী স্টাডি প্ল্যান আর কবে প্রিমিয়াম কিনবে](#পার্ট-৮-মাস-অনুযায়ী-স্টাডি-প্ল্যান-আর-কবে-প্রিমিয়াম-কিনবে)
- [সোর্স](#সোর্স)
- [কন্ট্রিবিউট করা](#কন্ট্রিবিউট-করা)

---

## ফ্লো না ভেঙে TryHackMe ফ্রি-তে যেভাবে ব্যবহার করবে

- **AttackBox না, নিজের Kali/Parrot VM + OpenVPN ব্যবহার করো।** ফ্রি অ্যাকাউন্টে AttackBox দিনে ১ ঘণ্টা লিমিটেড, কিন্তু OpenVPN দিয়ে নিজের মেশিন কানেক্ট করা আনলিমিটেড এবং ফ্রি।
- **পাথ ধরে না গিয়ে, নিচে দেওয়া ফ্রি রুম অর্ডার ধরো।** প্রতিটা রুম পেজে "Free" বা "Subscription" ব্যাজ দেখা যায়, আর রুম সার্চে "Free" ফিল্টার আছে।
- **ফ্রি অ্যাকাউন্টেও স্ট্রিক আর ব্যাজ কাউন্ট হয়।** প্রতিদিন একটা রুম বা টাস্ক করার অভ্যাস বানাও।
- **প্রিমিয়াম রুমে আটকে গেলে স্কিপ করে পরের ফ্রি রুমে যাও।** প্রতিটা পার্টে প্রিমিয়াম রুম আলাদা লিস্টে দেওয়া আছে, সাবস্ক্রিপশন নিলে এক মাসেই শেষ করা যাবে।
- **নোট রাখো (Obsidian, Notion, বা নিজের একটা প্রাইভেট GitHub রিপো)।** প্রতিটা কমান্ড আর মেথডলজি লিখে রাখো — প্রফেশনাল লেভেলে এই নোটগুলোই তোমার রিপোর্ট-রাইটিং টুলকিট হয়ে যাবে।

> রুমের ফ্রি/প্রিমিয়াম স্ট্যাটাস মাঝেমধ্যে বদলায়। রুম খোলার আগে ব্যাজ চেক করো, আর কিছু বদলে গেলে এই রিপোতে ইস্যু/পিআর দিয়ে জানাও।

---

## পার্ট ১: একদম বেসিক (Pre Security) — ২ সপ্তাহ

**Pre Security পাথ ১০০% ফ্রি**, তাই এখান থেকেই শুরু করো। গোল: সাইবার সিকিউরিটি কী, নেটওয়ার্ক আর ওয়েব কীভাবে কাজ করে, আর Linux ও Windows-এর বেসিক কমান্ড শেখা।

### ফ্রি রুম (এই অর্ডারে করো)

| # | রুম | কী শিখবে |
| --- | --- | --- |
| ১ | [Offensive Security Intro](https://tryhackme.com/room/offensivesecurityintro) | প্রথম হ্যাক — একটা ফেক ব্যাংক অ্যাপে Gobuster দিয়ে হিডেন পেজ খোঁজা |
| ২ | [Defensive Security Intro](https://tryhackme.com/room/defensivesecurityintro) | SOC, SIEM, ব্লু টিম বেসিক্স |
| ৩ | Careers in Cyber | পেনটেস্টার, SOC অ্যানালিস্ট, রেড টিমার — কোন পথে যাবে |
| ৪ | [What is Networking?](https://tryhackme.com/room/whatisnetworking) | IP, MAC, ping |
| ৫ | Intro to LAN | টপোলজি, সাবনেট, ARP, DHCP |
| ৬ | OSI Model | ৭ লেয়ার — ইন্টারভিউতে সবসময় আসে |
| ৭ | Packets & Frames | TCP হ্যান্ডশেক, পোর্ট |
| ৮ | Extending Your Network | NAT, ফায়ারওয়াল, VPN |
| ৯ | [DNS in Detail](https://tryhackme.com/room/dnsindetail) | ডোমেইন কীভাবে রিজলভ হয় |
| ১০ | [HTTP in Detail](https://tryhackme.com/room/httpindetail) | রিকোয়েস্ট, রেসপন্স, হেডার, কুকি |
| ১১ | [How Websites Work](https://tryhackme.com/room/howwebsiteswork) | HTML/JS, প্রথম XSS-এর স্বাদ |
| ১২ | [Putting it all together](https://tryhackme.com/room/puttingitalltogether) | লোড ব্যালান্সার, CDN, WAF |
| ১৩ | [Linux Fundamentals Part 1](https://tryhackme.com/room/linuxfundamentalspart1) | ls, cd, cat, find, grep |
| ১৪ | [Linux Fundamentals Part 2](https://tryhackme.com/room/linuxfundamentalspart2) | SSH, পারমিশন, ফ্ল্যাগ |
| ১৫ | [Linux Fundamentals Part 3](https://tryhackme.com/room/linuxfundamentalspart3) | Cron, প্যাকেজ, লগ |
| ১৬ | [Windows Fundamentals 1](https://tryhackme.com/room/windowsfundamentals1xbx) | ফাইল সিস্টেম, UAC, ইউজার |
| ১৭ | [Windows Fundamentals 2](https://tryhackme.com/room/windowsfundamentals2x0x) | msconfig, রেজিস্ট্রি, টাস্ক ম্যানেজার |
| ১৮ | [Windows Fundamentals 3](https://tryhackme.com/room/windowsfundamentals3xzx) | Defender, ফায়ারওয়াল, BitLocker |

### এই লেভেলে প্রিমিয়াম রুম

কোনোটাই নেই — Pre Security সম্পূর্ণ ফ্রি। পাথ কমপ্লিট করলে প্রথম সার্টিফিকেট পাবে, যেটা LinkedIn-এ দেওয়া যায়।

**অপশনাল ফ্রি এক্সট্রা:** [Search Skills](https://tryhackme.com/room/searchskills), Tutorial, OpenVPN রুম (নিজের VM কানেক্ট করার জন্য)।

---

## পার্ট ২: ফান্ডামেন্টালস আর টুলিং (Cyber Security 101 লেভেল) — ৩ সপ্তাহ

এখানে প্রথম পেওয়াল আসে: **Cyber Security 101** পাথের প্রায় অর্ধেক রুম প্রিমিয়াম। তাই পাথ না ধরে নিচের ফ্রি অর্ডার ধরো — একই টপিক কভার হয়ে যাবে।

### ফ্রি রুম

| # | রুম | টপিক |
| --- | --- | --- |
| ১ | [Introductory Networking](https://tryhackme.com/room/introtonetworking) | OSI/TCP-IP রিক্যাপ, ping, traceroute, whois, dig |
| ২ | [Network Services](https://tryhackme.com/room/networkservices) | SMB, Telnet, FTP এনুমারেট + এক্সপ্লয়েট |
| ৩ | [Network Services 2](https://tryhackme.com/room/networkservices2) | NFS, SMTP, MySQL |
| ৪ | [Nmap](https://tryhackme.com/room/furthernmap) | পুরো Nmap — স্ক্যান টাইপ, স্ক্রিপ্ট |
| ৫ | Nmap Live Host Discovery | ARP/ICMP হোস্ট ডিসকভারি |
| ৬ | [Passive Reconnaissance](https://tryhackme.com/room/passiverecon) | whois, nslookup, Shodan |
| ৭ | [Active Reconnaissance](https://tryhackme.com/room/activerecon) | ব্রাউজার ডেভ টুলস, ping, telnet |
| ৮ | Traffic Analysis Essentials | প্যাকেট কী, কীভাবে দেখে |
| ৯ | [Encryption - Crypto 101](https://tryhackme.com/room/encryptioncrypto101) | RSA, SSH কী, GPG |
| ১০ | [Crack the Hash](https://tryhackme.com/room/crackthehash) | Hashcat/John হ্যান্ডস-অন |
| ১১ | [Hydra](https://tryhackme.com/room/hydra) | SSH/ওয়েব লগইন ব্রুট ফোর্স |
| ১২ | Bash Scripting | অটোমেশন বেসিক |
| ১৩ | Python Basics | টুল লেখার জন্য |
| ১৪ | Regular Expressions | লগ/গ্রেপে রেজেক্স |

### প্রিমিয়াম রুম (Cyber Security 101) — এবং ফ্রি-তে যেভাবে কভার হয়

| প্রিমিয়াম রুম | টপিক | ফ্রি-তে কভার হয় যে রুমে |
| --- | --- | --- |
| Windows Command Line | cmd বেসিক্স | Windows Fundamentals 1-3 + নিজের PC-তে প্র্যাকটিস |
| Windows PowerShell | PowerShell বেসিক্স | Microsoft Learn PowerShell মডিউল (ফ্রি) |
| Linux Shells | Bash শেল স্ক্রিপ্টিং | Bash Scripting রুম (ফ্রি) |
| Networking Concepts / Essentials / Core Protocols / Secure Protocols | মডার্ন নেটওয়ার্কিং মডিউল | Introductory Networking + পার্ট ১-এর নেটওয়ার্ক রুম |
| Wireshark: The Basics | প্যাকেট অ্যানালাইসিস GUI | Traffic Analysis Essentials + নিজে Wireshark ইনস্টল করে প্র্যাকটিস |
| Tcpdump: The Basics | CLI প্যাকেট ক্যাপচার | Wireshark-এর পর নিজে ট্রাই করো |
| Nmap: The Basics | Nmap ইন্ট্রো | ফ্রি Nmap রুম (আরও ডিটেইলড) |
| Cryptography Basics / Public Key Crypto / Hashing Basics | ক্রিপ্টো থিওরি | Encryption - Crypto 101 + Crack the Hash |
| John the Ripper: The Basics | পাসওয়ার্ড ক্র্যাকিং | Crack the Hash (ফ্রি) |
| Gobuster: The Basics | ডিরেক্টরি ব্রুট ফোর্স | পার্ট ৩-এর Content Discovery |
| Shells Overview | রিভার্স/বাইন্ড শেল | পার্ট ৪-এর What the Shell? |
| SQLMap: The Basics | অটো SQLi | পার্ট ৩-এর SQL Injection রুম |
| CyberChef / CAPA / REMnux / FlareVM | ডিফেন্সিভ টুলিং | CyberChef সাইট নিজে ব্যবহার করো |

---

## পার্ট ৩: ওয়েব অ্যাপ্লিকেশন হ্যাকিং — ৪ সপ্তাহ

TryHackMe-তে ওয়েব হ্যাকিং-এর ফ্রি কনটেন্ট সবচেয়ে বেশি। Jr Penetration Tester পাথের ওয়েব মডিউলের দরকার নেই — ফ্রি রুম দিয়েই পুরো OWASP Top 10 কভার হয়ে যায়।

### ফ্রি রুম

| # | রুম | টপিক |
| --- | --- | --- |
| ১ | [Web Application Basics](https://tryhackme.com/room/webapplicationbasics) | URL, হেডার, মেথড, স্ট্যাটাস কোড |
| ২ | [Walking An Application](https://tryhackme.com/room/walkinganapplication) | ডেভ টুলস দিয়ে ম্যানুয়াল রিকন |
| ৩ | Content Discovery | robots.txt, Gobuster, ffuf |
| ৪ | Subdomain Enumeration | OSINT, ব্রুট ফোর্স, vhost |
| ৫ | Authentication Bypass | ইউজারনেম এনুম, লজিক ফ্ল |
| ৬ | IDOR | ইনসিকিউর ডাইরেক্ট অবজেক্ট রেফারেন্স |
| ৭ | [File Inclusion](https://tryhackme.com/room/filepathtraversal) | LFI/RFI, পাথ ট্রাভার্সাল |
| ৮ | [SSRF](https://tryhackme.com/room/ssrfhr) | সার্ভার সাইড রিকোয়েস্ট ফরজারি |
| ৯ | [XSS](https://tryhackme.com/room/axss) | রিফ্লেক্টেড, স্টোরড, DOM |
| ১০ | Command Injection | OS কমান্ড ইনজেক্ট |
| ১১ | [SQL Injection](https://tryhackme.com/room/sqlinjectionlm) | ইন-ব্যান্ড, ব্লাইন্ড, ইউনিয়ন |
| ১২ | [OWASP Top 10 - 2021](https://tryhackme.com/room/owasptop102021) | সব ১০টা একসাথে হ্যান্ডস-অন |
| ১৩ | [Burp Suite: The Basics](https://tryhackme.com/room/burpsuitebasics) | প্রক্সি, টার্গেট, ইন্টারসেপ্ট |
| ১৪ | [Burp Suite: Repeater](https://tryhackme.com/room/burpsuiterepeater) | রিকোয়েস্ট মডিফাই করে রিসেন্ড |
| ১৫ | [Introduction to OWASP ZAP](https://tryhackme.com/room/learnowaspzap) | Burp-এর ফ্রি অলটারনেটিভ |
| ১৬ | [OWASP Juice Shop](https://tryhackme.com/room/owaspjuiceshop) | রিয়েল অ্যাপে OWASP প্র্যাকটিস |
| ১৭ | [CSRF](https://tryhackme.com/room/csrfV2) | ক্রস-সাইট রিকোয়েস্ট ফরজারি |
| ১৮ | [NoSQL Injection](https://tryhackme.com/room/nosqlinjectiontutorial) | MongoDB ইনজেক্ট |
| ১৯ | [OWASP Broken Access Control](https://tryhackme.com/room/owaspbrokenaccesscontrol) | অ্যাক্সেস কন্ট্রোল বাইপাস |
| ২০ | [Advanced SQL Injection](https://tryhackme.com/room/advancedsqlinjection) | সেকেন্ড-অর্ডার, আউট-অফ-ব্যান্ড |
| ২১ | [DVWA](https://tryhackme.com/room/dvwa) / [WebGOAT](https://tryhackme.com/room/webgoat) | প্র্যাকটিস প্লেগ্রাউন্ড |

**ফ্রি ওয়েব CTF:** [Overpass](https://tryhackme.com/room/overpass), [Bolt](https://tryhackme.com/room/bolt), Takeover, Corridor, [Pickle Rick](https://tryhackme.com/room/picklerick), [RootMe](https://tryhackme.com/room/rrootme)।

### প্রিমিয়াম রুম (Jr Pentester ওয়েব মডিউল) — এবং ফ্রি-তে কভারেজ

| প্রিমিয়াম রুম | টপিক | ফ্রি-তে কভার হয় যেভাবে |
| --- | --- | --- |
| Burp Suite: Intruder / Other Modules / Extensions | অ্যাডভান্সড Burp | PortSwigger Web Security Academy-এর Burp ল্যাব (ফ্রি) |
| Web Enumeration / Web Recon মডিউল | স্ট্রাকচার্ড রিকন | Content Discovery + Subdomain Enumeration |
| Race Conditions | রেস কন্ডিশন | PortSwigger Academy রেস কন্ডিশন ল্যাব |
| XXE Injection | XML এক্সটার্নাল এনটিটি | PortSwigger Academy XXE ল্যাব |
| Insecure Deserialization | অবজেক্ট ইনজেক্ট | PortSwigger Academy ডিসিরিয়ালাইজেশন ল্যাব |
| API Testing / Broken Authentication (2025 মডিউল) | API সিকিউরিটি | PortSwigger API ল্যাব + OWASP crAPI |
| Web Application Pentesting ক্যাপস্টোন | এন্ড-টু-এন্ড চ্যালেঞ্জ | উপরের ফ্রি CTF লিস্ট |

> ওয়েবের জন্য **PortSwigger Web Security Academy** (portswigger.net/web-security) সম্পূর্ণ ফ্রি এবং TryHackMe প্রিমিয়ামের চেয়েও গভীর — ওয়েব প্রিমিয়াম স্কিপ করলে কোনো ক্ষতি নেই।

---

## পার্ট ৪: এক্সপ্লয়টেশন টুলস আর প্রথম মেশিনগুলো — ৪ সপ্তাহ

এই পার্টে তুমি প্রথমবার পুরো চেইন চালাবে: **স্ক্যান → এনুমারেট → এক্সপ্লয়েট → শেল**। Jr Penetration Tester পাথের "Vulnerability Research" আর "Metasploit" মডিউলের মূল রুমগুলো ফ্রি।

### ফ্রি রুম

| # | রুম | টপিক |
| --- | --- | --- |
| ১ | [Vulnerabilities 101](https://tryhackme.com/room/vulnerabilities101) | CVE, CVSS, NVD, Exploit-DB |
| ২ | Exploit Vulnerabilities | Searchsploit, ম্যানুয়াল এক্সপ্লয়েট |
| ৩ | [Metasploit: Introduction](https://tryhackme.com/room/metasploitintro) | msfconsole, মডিউল |
| ৪ | Metasploit: Exploitation | স্ক্যান + এক্সপ্লয়েট + msfvenom |
| ৫ | Metasploit: Meterpreter | পোস্ট-এক্সপ্লয়টেশন শেল |
| ৬ | [What the Shell?](https://tryhackme.com/room/introtoshells) | রিভার্স/বাইন্ড শেল, netcat, শেল স্টেবিলাইজ |
| ৭ | Protocols and Servers 1 & 2 | FTP/SMTP/POP3/IMAP অ্যাটাক + সিকিউর ভার্সন |
| ৮ | [Hydra](https://tryhackme.com/room/hydra) (রিক্যাপ) | ব্রুট ফোর্স লগইন |
| ৯ | Common Linux Privesc | প্রথম প্রিভেস্কের স্বাদ |

### প্রথম ৮টা মেশিন (ফ্রি, এই অর্ডারে)

| # | রুম | কেন |
| --- | --- | --- |
| ১ | [Vulnversity](https://tryhackme.com/room/vulnversity) | Nmap + Gobuster + আপলোড বাইপাস + প্রিভেস্ক — পুরো চেইন |
| ২ | [Blue](https://tryhackme.com/room/blue) | EternalBlue দিয়ে Windows হ্যাক, Metasploit |
| ৩ | [Simple CTF](https://tryhackme.com/room/easyctf) | CVE খুঁজে এক্সপ্লয়েট করা |
| ৪ | [Bounty Hacker](https://tryhackme.com/room/cowboyhacker) | FTP anonymous + Hydra + sudo প্রিভেস্ক |
| ৫ | Brute It | Hydra + John + প্রিভেস্ক |
| ৬ | [Kenobi](https://tryhackme.com/room/kenobi) | Samba + ProFTPD + SUID |
| ৭ | [RootMe](https://tryhackme.com/room/rrootme) | আপলোড বাইপাস + SUID python |
| ৮ | Agent Sudo / Lazy Admin | স্টেগানোগ্রাফি + CMS এক্সপ্লয়েট |

### প্রিমিয়াম রুম (Jr Pentester) — এবং ফ্রি-তে কভারেজ

| প্রিমিয়াম রুম | টপিক | ফ্রি-তে কভার হয় যেভাবে |
| --- | --- | --- |
| Pentesting Fundamentals / Principles of Security | মেথডলজি, rules of engagement | Careers in Cyber + OWASP Testing Guide (ফ্রি PDF) |
| Passive/Active Recon (2026 রিবিল্ট ভার্সন) | রিকন | পুরনো ফ্রি Passive/Active Reconnaissance রুম |
| Net Sec Challenge | Nmap চ্যালেঞ্জ মেশিন | Nmap রুম + Vulnversity |
| Shells Overview / Enumeration & Brute Force | শেল + এনুম | What the Shell? (ফ্রি) |
| Metasploit: Post Exploitation (নতুন) | পার্সিস্টেন্স, পিভোটিং | Meterpreter রুম (ফ্রি) + Metasploit ডকস |
| Jr Pentester ক্যাপস্টোন (২০২৬-এ নতুন ৩টা) | এন্ড-টু-এন্ড | উপরের ফ্রি মেশিন লিস্ট |

---

## পার্ট ৫: প্রিভিলেজ এস্কেলেশন, অ্যাক্টিভ ডিরেক্টরি আর CTF প্র্যাকটিস — ৬ সপ্তাহ

এখন তুমি ইন্টারমিডিয়েট। প্রিভেস্ক আর AD-র মূল রুমগুলো ফ্রি — এখানে সবচেয়ে বেশি সময় দাও, কারণ এগুলোই PT1 আর OSCP দুটোতেই লাগবে।

### ফ্রি রুম — প্রিভিলেজ এস্কেলেশন

| # | রুম | টপিক |
| --- | --- | --- |
| ১ | [Linux Privilege Escalation](https://tryhackme.com/room/linprivesc) | কার্নেল, sudo, SUID, cron, PATH, NFS — পুরোটা |
| ২ | [Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | পুরনো ভার্সন, এক্সট্রা প্র্যাকটিস |
| ৩ | [Linux PrivEsc Arena](https://tryhackme.com/room/linuxprivescarena) | ২০+ প্রিভেস্ক প্র্যাকটিস |
| ৪ | [Windows PrivEsc](https://tryhackme.com/room/windows10privesc) | সার্ভিস, রেজিস্ট্রি, টোকেন, DLL |
| ৫ | [Windows PrivEsc Arena](https://tryhackme.com/room/windowsprivescarena) | Windows প্র্যাকটিস |
| ৬ | [Sudo Security Bypass](https://tryhackme.com/room/sudovulnsbypass) / [Sudo Buffer Overflow](https://tryhackme.com/room/sudovulnsbof) | CVE বেসড প্রিভেস্ক |
| ৭ | [Linux Agency](https://tryhackme.com/room/linuxagency) | ৩০+ লেভেল Linux প্রিভেস্ক ম্যারাথন |

### ফ্রি রুম — অ্যাক্টিভ ডিরেক্টরি

| # | রুম | টপিক |
| --- | --- | --- |
| ১ | [Active Directory Basics](https://tryhackme.com/room/winadbasics) | ডোমেইন, OU, GPO, Kerberos |
| ২ | [Breaching Active Directory](https://tryhackme.com/room/breachingad) | NTLM, LDAP, পাসওয়ার্ড স্প্রে |
| ৩ | [Attacktive Directory](https://tryhackme.com/room/attacktivedirectory) | Kerbrute + AS-REP roast + secretsdump |
| ৪ | [Post-Exploitation Basics](https://tryhackme.com/room/postexploit) | BloodHound, Mimikatz |
| ৫ | [Enterprise](https://tryhackme.com/room/enterprise) / [RazorBlack](https://tryhackme.com/room/raz0rblack) | মিডিয়াম AD বক্স |
| ৬ | [Active Directory Hardening](https://tryhackme.com/room/activedirectoryening) | ডিফেন্স সাইড |

### ফ্রি CTF গ্রাইন্ড (প্রতিদিন একটা করে)

- **Easy:** [Blaster](https://tryhackme.com/room/blaster), Ignite, Startup, Lian Yu, Break Out The Cage, B3dr0ck, Anthem, Blueprint, Retro
- **Medium:** [Mr Robot CTF](https://tryhackme.com/room/mrrobot), [GoldenEye](https://tryhackme.com/room/goldeneye), [Wonderland](https://tryhackme.com/room/wonderland), [Relevant](https://tryhackme.com/room/relevant), Dogcat, VulnNet: Active, Ollie, Eavesdropper
- **Buffer overflow (OSCP-স্টাইল):** [Buffer Overflow Prep](https://tryhackme.com/room/bufferoverflowprep), [Gatekeeper](https://tryhackme.com/room/gatekeeper), [Intro To Pwntools](https://tryhackme.com/room/introtopwntools)

### এই লেভেলে প্রিমিয়াম রুম — এবং ফ্রি-তে কভারেজ

| প্রিমিয়াম রুম | টপিক | ফ্রি-তে কভার হয় যেভাবে |
| --- | --- | --- |
| Intro to AD Breaching / Authenticated Enumeration / Credential Harvesting / Lateral Movement (2026 Jr Pentester AD মডিউল) | স্ট্রাকচার্ড AD অ্যাটাক চেইন | Breaching AD + Post-Exploitation Basics + Attacktive Directory |
| Active Directory Challenge 1 (নতুন) | AD ক্যাপস্টোন | Enterprise, RazorBlack |
| Enumerating / Lateral Movement & Pivoting / Exploiting / Persisting AD (Red Team পাথ) | ডিপ AD | উপরের ফ্রি AD লিস্ট + HackTheBox ফ্রি AD বক্স |
| Wreath | নেটওয়ার্ক পিভোটিং | ফ্রি অলটারনেটিভ নেই — সবচেয়ে ভ্যালুয়েবল প্রিমিয়াম রুম, সাবস্ক্রিপশন নিলে প্রথমে এটা করো |
| Holo | AD নেটওয়ার্ক সিমুলেশন | Wreath-এর পর |
| Throwback | AD নেটওয়ার্ক | Holo-এর পর |

---

## পার্ট ৬: প্রফেশনাল লেভেল — স্পেশালাইজেশন আর সার্টিফিকেশন

পার্ট ৫ শেষ করলে তুমি এন্ট্রি-লেভেল জব রেডি। এখন একটা লেন বাছতে হবে: **রেড টিম (পেনটেস্টিং)** নাকি **ব্লু টিম (SOC)**। দুটোই TryHackMe-তে আছে, কিন্তু এই লেভেলের পাথগুলো বেশিরভাগ প্রিমিয়াম — এখানে এক মাস সাবস্ক্রিপশন নিলে টাকা উশুল হয়।

### রেড টিম লেন

| পাথ | ফ্রি/প্রিমিয়াম | নোট |
| --- | --- | --- |
| Jr Penetration Tester (৮৯ রুম, ১৭ মডিউল, ~৭০-৯০ ঘণ্টা) | মিক্সড, ~৪০% ফ্রি | পার্ট ৩-৫-এর ফ্রি রুম দিয়ে অর্ধেক আগেই শেষ; প্রিমিয়াম অংশ ১ মাসে শেষ হয় |
| Offensive Pentesting | বেশিরভাগ প্রিমিয়াম | ফ্রি: [Kenobi](https://tryhackme.com/room/kenobi), [Blue](https://tryhackme.com/room/blue), [Relevant](https://tryhackme.com/room/relevant), Buffer Overflow Prep, Attacktive Directory, Gatekeeper |
| Red Teaming | বেশিরভাগ প্রিমিয়াম | ফ্রি: [Red Team Recon](https://tryhackme.com/room/redteamrecon), [Red Team OPSEC](https://tryhackme.com/room/opsec), Red Team Fundamentals, Intro to Antivirus |

### ব্লু টিম লেন

| পাথ | ফ্রি/প্রিমিয়াম | নোট |
| --- | --- | --- |
| SOC Level 1 | মিক্সড | ফ্রি: Snort, Traffic Analysis Essentials, Windows Forensics 1, Linux Process Analysis, Phishing Analysis, Threat Hunting: Foothold + ৪০+ ফ্রি ফরেনসিক্স রুম |
| SOC Level 2 | প্রিমিয়াম | SAL2-এর জন্য |
| Cyber Defense | মিক্সড | ফ্রি ফরেনসিক্স/লগ অ্যানালাইসিস রুম দিয়ে বড় অংশ কভার হয় |

### সার্টিফিকেশন অর্ডার (এই সিকোয়েন্সে)

| সার্টিফিকেট | কার জন্য | ফরম্যাট | দাম (USD) | কী লাগবে আগে |
| --- | --- | --- | --- | --- |
| SEC0 (Pre-Security) | কমপ্লিট বিগিনার | প্র্যাকটিক্যাল টাস্ক | কম দাম, SEC1-এর সাথে বান্ডেলে ২০% ছাড় | পার্ট ১ |
| SEC1 (Security 101) | ফাউন্ডেশন প্রুফ | প্র্যাকটিক্যাল অ্যাসেসমেন্ট | প্রিমিয়ামে ১৫% ছাড় | পার্ট ২ |
| PT1 (Junior Penetration Tester) | রেড টিম এন্ট্রি | ৪৮ ঘণ্টা প্র্যাকটিক্যাল + রিপোর্ট | $২৯৭ (৩ মাস প্রিমিয়াম + ১ রিটেক সহ) | পার্ট ৩-৫ + Jr Pentester পাথ |
| SAL1 (Security Analyst Level 1) | SOC এন্ট্রি | লাইভ SOC সিমুলেটর + ইনসিডেন্ট রিপোর্ট | $৩৪৯ (৩ মাস প্রিমিয়াম + ১ রিটেক সহ) | SOC Level 1 পাথ |
| SAL2 | মিড-লেভেল SOC | মাল্টি-স্টেজ ইনভেস্টিগেশন | প্রিমিয়ামে ১৫% ছাড় | SAL1 |
| AI1 (AI Security) | স্পেশালিস্ট | ১৩টা হ্যান্ডস-অন সিনারিও | প্রিমিয়ামে ১৫% ছাড় | PT1 বা SAL1 |

PT1/SAL1-এর ভ্যালিডিটি ৩ বছর, এক্সাম অ্যাটেম্পট কেনার থেকে ১২ মাসের মধ্যে দিতে হয়। **সবচেয়ে কস্ট-এফেক্টিভ রুট:** PT1 ($২৯৭) কিনলেই ৩ মাস প্রিমিয়াম ফ্রি পাওয়া যায় — তাই আলাদা সাবস্ক্রিপশন না কিনে সার্টিফিকেট কেনো, একসাথে সব প্রিমিয়াম রুম আর এক্সাম পাওয়া যাবে।

### TryHackMe-এর বাইরের প্রফেশনাল সার্টিফিকেট

| সার্টিফিকেট | দাম | কখন |
| --- | --- | --- |
| eJPT (INE) | ~$২৫০ | PT1-এর অলটারনেটিভ, HR-এ বেশি চেনা |
| CompTIA Security+ | ~$৪০০ | ব্লু টিম জবের জন্য HR ফিল্টার পাস করতে |
| OSCP (OffSec) | ~$১,৭৫০ | ১-২ বছর পরে, পার্ট ৫-এর বাফার ওভারফ্লো + AD শেষ করে |
| CPTS (HackTheBox) | ~$২১০ | OSCP-এর চেয়ে সস্তা ও কঠিন অলটারনেটিভ |

> আমি আইনজীবী/ফাইনান্সিয়াল অ্যাডভাইজার না — দামগুলো ২০২৬ সেপ্টেম্বরের, কেনার আগে অফিসিয়াল সাইটে চেক করে নাও।

---

## পার্ট ৭: প্রতিটি প্রিমিয়াম টপিকের ফ্রি অলটারনেটিভ

| প্রিমিয়াম টপিক | ফ্রি অলটারনেটিভ | লিংক |
| --- | --- | --- |
| Burp অ্যাডভান্সড, XXE, ডিসিরিয়ালাইজেশন, রেস কন্ডিশন, API | PortSwigger Web Security Academy — ২০০+ ল্যাব, সম্পূর্ণ ফ্রি | portswigger.net/web-security |
| Wireshark / Tcpdump | Wireshark ইনস্টল করে malware-traffic-analysis.net-এর pcap এক্সারসাইজ | malware-traffic-analysis.net |
| Wreath / Holo / Throwback (নেটওয়ার্ক পিভোটিং, AD) | HackTheBox ফ্রি রিটায়ার্ড মেশিন + HTB Academy ফ্রি টিয়ার; নিজে GOAD (Game of AD) ল্যাব বানাও | hackthebox.com, github.com/Orange-Cyberdefense/GOAD |
| Windows CLI / PowerShell | Microsoft Learn PowerShell মডিউল | learn.microsoft.com/powershell |
| Red Team পাথ (C2, evasion) | The Cyber Mentor (TCM)-এর ফ্রি YouTube কোর্স, MalDev Academy-এর ফ্রি অংশ | youtube.com/@TCMSecurityAcademy |
| SOC Level 1 প্রিমিয়াম (SIEM, Splunk) | Splunk Boss of the SOC (BOTS) ফ্রি ডেটাসেট, LetsDefend ফ্রি টিয়ার, CyberDefenders ফ্রি চ্যালেঞ্জ | letsdefend.io, cyberdefenders.org |
| Metasploit পোস্ট-এক্সপ্লয়টেশন | OffSec Metasploit Unleashed (ফ্রি) | offsec.com/metasploit-unleashed |
| OSCP-স্টাইল প্র্যাকটিস বক্স | VulnHub (ফ্রি ডাউনলোড, অফলাইন VM) | vulnhub.com |

**নিয়ম:** এক প্ল্যাটফর্মে আটকে গেলে অন্য প্ল্যাটফর্মে একই টপিক করো, কিন্তু **মূল ট্র্যাক TryHackMe-এর ফ্রি লিস্ট** — নাহলে সব জায়গায় আধা-আধি হয়ে যাবে।

---

## পার্ট ৮: মাস অনুযায়ী স্টাডি প্ল্যান আর কবে প্রিমিয়াম কিনবে

দিনে ১.৫-২ ঘণ্টা দিলে ৬ মাসে পার্ট ১-৫ ফ্রি-তে শেষ হয়, ৭-৮ মাসে PT1-এর জন্য রেডি হয়ে যাবে।

| মাস | কী করবে | ফ্রি/প্রিমিয়াম |
| --- | --- | --- |
| ১ | পুরো পার্ট ১ (Pre Security) + Kali VM + OpenVPN সেটআপ + নোট সিস্টেম | ফ্রি |
| ২ | পার্ট ২-এর ফ্রি রুম + Bash/Python বেসিক | ফ্রি |
| ৩ | পার্ট ৩-এর ওয়েব রুম (১-১৬) + PortSwigger Academy-এর SQLi/XSS ল্যাব | ফ্রি |
| ৪ | পার্ট ৩-এর বাকিটা + পার্ট ৪-এর টুলস + প্রথম ৮টা মেশিন | ফ্রি |
| ৫ | পার্ট ৫-এর প্রিভেস্ক (Linux + Windows) + প্রতিদিন ১টা easy CTF | ফ্রি |
| ৬ | পার্ট ৫-এর AD + medium CTF + বাফার ওভারফ্লো | ফ্রি |
| ৭ | **প্রিমিয়াম/PT1 কেনো** — Jr Pentester পাথের প্রিমিয়াম রুম + Wreath + Holo + ক্যাপস্টোন | প্রিমিয়াম (PT1-এর সাথে ৩ মাস ফ্রি) |
| ৮ | PT1 এক্সাম + রিপোর্ট প্র্যাকটিস; SOC লেন হলে SOC Level 1-এর প্রিমিয়াম রুম | প্রিমিয়াম |
| ৯+ | লেন অনুযায়ী: Red Teaming পাথ / SOC Level 2, HackTheBox, eJPT বা OSCP প্রেপ | মিক্সড |

### প্রিমিয়াম কেনা উচিত কি না?

- **এখন না।** পার্ট ১-৫-এ ৩০০+ ফ্রি রুম আছে — শেষ করতে ৬ মাস লাগবে। এখন কিনলে বেশিরভাগ মাসে প্রিমিয়াম রুম খুলবে না, টাকা নষ্ট।
- **৭ নম্বর মাসে কিনো, সাবস্ক্রিপশন না কিনে PT1 এক্সাম কিনো ($২৯৭)।** এতে ৩ মাস প্রিমিয়াম ফ্রি পাওয়া যায় — মাসিক $১৬.৯৯ করে ৩ মাসে $৫১ যেত, এক্সামের সাথে সেটা কভার হয়ে যায়।
- শুধু সাবস্ক্রিপশন লাগলে **অ্যানুয়াল স্টুডেন্ট প্ল্যান** ($৮.৩৩/মাস, .edu ইমেইল লাগবে) — ইউনিভার্সিটি ইমেইল থাকলে ব্যবহার করো।
- প্রিমিয়াম নিলে প্রথমে এই অর্ডারে করো: Wreath → Jr Pentester AD মডিউল → Holo → Throwback → ক্যাপস্টোন। এই ৫টা ফ্রি-তে নেই এবং সবচেয়ে জব-রিলেভ্যান্ট।

### প্রতিদিনের রুটিন

- [ ] ১টা রুম বা ১টা CTF (স্ট্রিক রাখো)
- [ ] নোটে কমান্ড + মেথডলজি যোগ করো
- [ ] সপ্তাহে ১ দিন: পুরনো CTF আবার নোট ছাড়া সলভ করো (রিটেনশন চেক)
- [ ] মাসে ১ বার: এই লিস্টের রুম ব্যাজ চেক করো — ফ্রি/প্রিমিয়াম বদলেছে কি না

---

## সোর্স

- [TryHackMe — Free TryHackMe Training: The Ultimate Guide for Beginners](https://tryhackme.com/resources/blog/free_path)
- [TryHackMe — Free Rooms](https://tryhackme.com/free-rooms)
- [TryHackMe — Jr Penetration Tester Learning Path Rebuilt for 2026](https://tryhackme.com/resources/blog/jr-penetration-tester-learning-path-rebuilt-for-2026)
- [TryHackMe — Certification Guide 2026](https://tryhackme.com/resources/blog/tryhackme-certification-guide)
- [HackerDNA — TryHackMe Certifications 2026: SAL1 & PT1 Cost + Validity](https://hackerdna.com/blog/tryhackme-certifications)
- [CertCompass — TryHackMe Review 2026](https://certcompass.org/tryhackme-review-2026/)
- [winterrdog/tryhackme-free-rooms](https://github.com/winterrdog/tryhackme-free-rooms)
- [Hunterdii/TryHackMe-Roadmap](https://github.com/Hunterdii/TryHackMe-Roadmap)

## কন্ট্রিবিউট করা

কোনো রুম ফ্রি থেকে প্রিমিয়াম হয়ে গেছে (বা উল্টো) দেখলে, রুমের লিংক আর চেক করার তারিখ দিয়ে একটা ইস্যু বা পুল রিকোয়েস্ট দাও। স্টার দিলে অন্য বিগিনাররা এই রোডম্যাপ খুঁজে পেতে সাহায্য হয়।

**কীওয়ার্ড:** TryHackMe roadmap Bangla, TryHackMe free rooms bangla, ট্রাইহ্যাকমি ফ্রি রুম লিস্ট, সাইবার সিকিউরিটি রোডম্যাপ বাংলা, ফ্রি এথিক্যাল হ্যাকিং শেখা, PT1 সার্টিফিকেশন স্টাডি প্ল্যান, SAL1 স্টাডি প্ল্যান, Jr Penetration Tester পাথ ফ্রি রুম, OSCP প্রিপারেশন।

## লাইসেন্স

MIT — ফর্ক করা, অনুবাদ করা, এবং attribution সহ শেয়ার করা যাবে, সম্পূর্ণ ফ্রি।
