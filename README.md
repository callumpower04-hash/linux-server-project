Secure Linux Server Project

A secure multi-VM Linux lab built as part of my Internet & Network Services module (MTU, 2025).
Designed to showcase skills in Linux server hardening, networking, and cybersecurity.
Achieved 78% grade for this project.

Project Overview

VM2 → SSH hardening, UFW firewall, CUPS print server, Bind9 Primary DNS

VM3 → DHCP server, Bind9 Secondary DNS, Postfix + Dovecot mail services, iSCSI storage target

Client → used for DNS/DHCP/iSCSI/Mail testing

Monitored using Netdata (screenshot included in /docs/)

Security Measures

Disabled root SSH login, key-based authentication only

UFW firewall: deny-all inbound, allow only required services

Role-based VM separation (DNS, DHCP, Mail, Storage) to reduce attack surface

Public repo sanitised (calmnet.local → example.local)

Repository Layout
configs/
  vm2/   → SSH, UFW, CUPS, Bind9 (Primary DNS)
  vm3/   → DHCP, Bind9 (Secondary DNS), Postfix/Dovecot, iSCSI
docs/
  vm2/   → Netdata monitoring screenshot

  
