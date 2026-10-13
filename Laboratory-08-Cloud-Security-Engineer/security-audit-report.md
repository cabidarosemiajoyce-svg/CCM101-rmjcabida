# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means giving each user or service only the permissions needed to perform its assigned tasks. This helps reduce the risk of unauthorized access and limits the damage that can occur if an account is compromised.

## 2. Attack Surface

The attack surface refers to the points where an attacker might try to access or exploit a system. On a virtual machine, this may include exposed network ports, running services, and accounts with weak security settings.

## 3. Default Deny Policy

A Default Deny policy blocks incoming network traffic unless a specific rule allows it. This is safer than trying to block individual attackers because it restricts unapproved connections, including connections from sources that have not yet been identified as malicious.

## 4. Application Test

The web application was tested using curl before configuring the firewall. The actual command and result will be recorded after the test is completed.

## 5. Firewall Audit Result

The UFW status, default policies, and permitted ports will be documented after configuring and verifying the firewall.
