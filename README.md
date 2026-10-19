# Linux Server Administration Project

## Overview
This project demonstrates the installation, configuration, and testing of three server services using Ubuntu 24.04 LTS on Windows Subsystem for Linux (WSL).

## Services Configured

### 1. Apache Web Server
- Installed Apache2.
- Created a custom HTML webpage.
- Tested the website using `curl`.
- Verified that Apache returned the custom HTML content.

### 2. BIND9 DNS Server
- Installed BIND9 and DNS utilities.
- Configured the `myschool.test` DNS zone.
- Created DNS records for `ns1.myschool.test` and `www.myschool.test`.
- Validated the configuration using `named-checkconf` and `named-checkzone`.
- Tested DNS resolution using `dig`.
- Confirmed that `www.myschool.test` resolves to `127.0.0.1`.

### 3. Postfix Mail Server
- Installed Postfix and Mailutils.
- Configured the mail server hostname as `mail.myschool.test`.
- Restricted Postfix to local connections.
- Sent a test email to the local Linux mailbox.

## Technologies Used
- Ubuntu Linux
- Windows Subsystem for Linux (WSL)
- Apache2
- BIND9
- Postfix
- HTML
- Linux command line

## Testing Results
- Apache served the custom HTML webpage.
- BIND9 successfully resolved the test domain.
- Postfix accepted a local test email, which appeared in the local mailbox.

## Environment and Limitations
This project runs in a local Ubuntu WSL environment. The `.test` domain is for testing and is not a public domain. The mail server is configured for local use and has not been configured as a publicly accessible email service.

## Author
Adelokiki
