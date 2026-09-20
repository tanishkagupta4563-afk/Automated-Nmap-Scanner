# Automated Nmap Scanner

![Bash](https://img.shields.io/badge/Bash-Scripting-black)
![Type](https://img.shields.io/badge/Tool-Network%20Reconnaissance-green)
![Security](https://img.shields.io/badge/Cybersecurity-Ethical%20Hacking-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## Overview

Automated Nmap Scanner is a Bash-based network reconnaissance tool that automates multiple Nmap scanning techniques into a single unified script.

It supports both interactive mode and command-line execution, making network scanning faster, structured, and easier to use for learning and lab environments.

This project is designed for cybersecurity students, ethical hacking practice, and authorized security testing only.

---

## Features

- Multiple Nmap scan types in one tool  
- Interactive + CLI-based execution  
- Automated scan execution  
- Structured output saving  
- Quick scan summary generation  
- Support for additional Nmap flags (`-T4`, `-p-`, etc.)  
- Lightweight and easy to use  

---

## Supported Scan Types

| Option | Scan Type | Nmap Flag |
|--------|----------|-----------|
| 1 | Host Discovery | `-sn` |
| 2 | TCP SYN Scan | `-sS` |
| 3 | UDP Scan | `-sU` |
| 4 | Version Detection | `-sV` |
| 5 | OS Detection | `-O` |
| 6 | All Scans | Full Execution |

---

## Requirements

- Linux / Unix-based system (Kali Linux recommended)  
- Nmap installed  

### Install Nmap
```bash
sudo apt update
sudo apt install nmap -y
````

---

## Installation

```bash
git clone https://github.com/tanishkagupta4563-afk/Automated-Nmap-Scanner.git
cd automated-nmap-scanner
chmod +x nmap_auto.sh
```

---

## Usage

### Run the tool

```bash
./nmap_auto.sh
```

---

### Steps

1. Enter target IP address or domain
2. Choose scan type (1–6)
3. Optional: Add extra Nmap flags

---

### Example

```text
Enter target IP / domain: scanme.nmap.org

Select scan type:
1. Host Discovery
2. TCP SYN Scan
3. UDP Scan
4. Version Detection
5. OS Detection
6. All Scans
```

---

## Output

All scan results are saved in:

```text
nmap_results.txt
```

The file contains:

* Full scan output
* Service and port information
* Scan-wise structured logs

---

## Sample Output

```text
Nmap scan report for scanme.nmap.org
22/tcp   open  ssh
80/tcp   open  http
443/tcp  open  https
```

---

## Scan Summary

At the end of execution, a quick summary is displayed:

```text
========= SCAN SUMMARY =========
open ports found
filtered ports found
closed ports found
```

---

## Security Notice

This tool is intended strictly for:

* Educational purposes
* Authorized testing
* Personal lab environments

Unauthorized scanning of systems without permission is illegal.

---

## Future Improvements

* Integration of Nmap NSE vulnerability scanning
* HTML/PDF report generation
* JSON export support
* Parallel scanning support
* Enhanced reporting dashboard

---

## Author

**Tanishka Gupta**

Secure Today. Safe Tomorrow.

