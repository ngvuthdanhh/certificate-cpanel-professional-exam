# Lab 01: Basic Setup of cPanel/WHM

## Goal
Install cPanel/WHM and complete the initial configuration wizard.

## Steps
1. Spin up a fresh CentOS/CloudLinux/AlmaLinux VM.
2. Run:
   ```bash
   cd /home && curl -o latest -L https://securedownloads.cpanel.net/latest && sh latest
   ```
Access WHM via https://<IP>:2087.

Complete setup wizard (hostname, nameservers, contact email).

## Check

Login to WHM successful.

Services (Apache, Exim, Dovecot) are running.
