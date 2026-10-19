# ShiftLedger — Web Exploitation Lab

A custom-built vulnerable web application lab designed for
offensive security practice and technical assessment.

## Overview

ShiftLedger simulates an internal payroll and shift-scheduling
portal for a fictional logistics company.

The project demonstrates how multiple security weaknesses can
be chained to escalate privileges from a low-privileged
employee account to root access on a Linux machine.

## Project Details

- **Project:** ShiftLedger
- **Category:** Web Application Security / Linux Privilege Escalation
- **Environment:** Ubuntu 24.04 LTS
- **Assessment Type:** Authenticated Web Exploitation
- **Testing Tools:** Burp Suite, ffuf, Python 3, Browser DevTools
- **Environment:** Authorized local lab

## Vulnerabilities Demonstrated

1. Mass Assignment
2. Broken Access Control and Improper Authorization
3. Server-Side Template Injection (SSTI)
4. Insecure Deserialization using Python Pickle
5. Linux Privilege Escalation through a Root-Running Service

## Attack Chain

Employee Account
       |
       v
Mass Assignment
       |
       v
Supervisor Privileges
       |
       v
Role Escalation
       |
       v
Finance Administrator
       |
       v
Server-Side Template Injection
       |
       v
Application Service Account
       |
       v
Insecure Deserialization
       |
       v
Root Access

## Methodology

- Reconnaissance and endpoint enumeration
- HTTP request and response analysis
- Authentication and authorization testing
- Input-handling and template-rendering analysis
- Privilege escalation analysis
- Impact assessment and remediation recommendations

## Tools Used

- Burp Suite
- ffuf
- Python 3
- Firefox / Chrome Developer Tools
- Linux command-line utilities

## Documentation

The assessment report includes the methodology, vulnerability
analysis, evidence, attack-chain milestones, and remediation
recommendations.

See [`docs/ShiftLedger_Writeup.pdf`](docs/ShiftLedger_Writeup.pdf).

## Security Notice

This project is intended for authorized security testing,
education, and isolated lab environments only.

Do not deploy the intentionally vulnerable application on a
public-facing server.

## Author

Mukund Ugale
