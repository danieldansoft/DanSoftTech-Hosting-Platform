\# DanSoftTech Infrastructure Lab — Real Validation



> \*\*REAL LABORATORY — BUILT, TESTED, VALIDATED AND DOCUMENTED\*\*



This document records the real infrastructure laboratory developed and operated by \*\*DanSoftTech \& Cobaltech\*\*.



The environment is based on physical equipment and real network services configured, tested and validated in the \*\*DanSoftTech Infrastructure Lab\*\*.



This is not a simulated infrastructure or a theoretical laboratory.



The configurations documented here were implemented on physical hardware and validated through real network, server, DNS, remote access, hosting and Cloudflare Tunnel tests.



\---



\## 🔬 Laboratory Identity



\*\*Project:\*\* DanSoftTech Infrastructure Lab  

\*\*Platform:\*\* DanSoftTech Hosting Platform  

\*\*Author:\*\* Daniel Cerri Ribeiro  

\*\*Organization:\*\* DanSoftTech \& Cobaltech  

\*\*Environment:\*\* Physical Infrastructure Laboratory  

\*\*Validation:\*\* Real Equipment • Real Network • Real Services



\---



\## 🎯 Laboratory Objective



The objective of this laboratory is to build, operate, test and document a complete infrastructure environment involving:



\- Windows Server 2025

\- MikroTik RouterOS

\- IPv4 networking

\- Public/Fixed IPv4 connectivity

\- Cloudflare DNS

\- Cloudflare Tunnel

\- Apache / XAMPP

\- Active Directory

\- OpenSSH / SFTP

\- VirtualHosts

\- Multi-site hosting

\- PowerShell automation

\- Remote administration

\- Network and service validation



The laboratory is continuously expanded as new technologies and infrastructure components are implemented and tested.



\---



\## 🟢 Current Laboratory Status



| Component | Status |

|---|---|

| Windows Server 2025 | 🟢 Operational |

| MikroTik RB2011 | 🟢 Operational |

| Public/Fixed IPv4 | 🟢 Validated |

| Cloudflare DNS | 🟢 Operational |

| Cloudflare Tunnel | 🟢 Operational |

| Apache / XAMPP | 🟢 Operational |

| Active Directory | 🟢 Configured |

| OpenSSH / SFTP | 🟢 Operational |

| VirtualHosts | 🟢 Tested |

| Multi-Site Hosting | 🟢 Validated |

| Remote Administration | 🟢 Tested |



\---



\# 🖥️ Physical Infrastructure



\## SERVER2025



The main server of the laboratory is a physical machine running:



\- Windows Server 2025 Datacenter

\- Kingston NVMe 1 TB

\- 16 GB RAM

\- Apache / XAMPP

\- Cloudflare Tunnel

\- Active Directory

\- OpenSSH / SFTP

\- Remote Desktop

\- UPS PW 2000

\- Controlled environment



\---



\## 💻 Management Station



\### AMD Ryzen 5 5600GT



The main management workstation includes:



\- AMD Ryzen 5 5600GT

\- 32 GB RAM

\- Windows 11 Pro

\- Visual Studio Code

\- FileZilla

\- PowerShell

\- Network administration tools



The workstation is used for administration, development, testing and validation of the laboratory infrastructure.



\---



\## 🌐 Network Infrastructure



The laboratory includes:



\- MikroTik RB2011

\- Huawei/ISP equipment

\- Ethernet infrastructure

\- Administrative network

\- Main LAN

\- IPv4 public connectivity

\- Remote administration

\- Cloudflare infrastructure



\---



\# 🧪 Real Laboratory Principle



The DanSoftTech Infrastructure Lab follows a simple engineering principle:



```



BUILD

&#x20; ↓

CONFIGURE

&#x20; ↓

TEST

&#x20; ↓

VALIDATE

&#x20; ↓

DOCUMENT

&#x20; ↓

PRESERVE EVIDENCE



```




\# 🌐 Real Network Topology



The DanSoftTech Infrastructure Lab uses a physical network architecture

integrating the ISP equipment, MikroTik RouterOS, SERVER2025 and the

management workstation.



```

&#x20;                        INTERNET

&#x20;                           │

&#x20;                           │

&#x20;                   PUBLIC / FIXED IPv4

&#x20;                           │

&#x20;                           ▼

&#x20;                   ISP / HUAWEI ROUTER

&#x20;                           │

&#x20;                           │

&#x20;                           ▼

&#x20;                    MIKROTIK RB2011

&#x20;                           │

&#x20;                ┌──────────┴──────────┐

&#x20;                │                     │

&#x20;                ▼                     ▼

&#x20;         MAIN NETWORK          ADMINISTRATION

&#x20;                │                     │

&#x20;                │                     │

&#x20;                ▼                     ▼

&#x20;            SERVER2025            SERVER2025

&#x20;         192.168.18.25          192.200.77.179

&#x20;                │

&#x20;                │

&#x20;                ▼

&#x20;          Apache / XAMPP

&#x20;                │

&#x20;                ▼

&#x20;       Cloudflare Tunnel

&#x20;                │

&#x20;                ▼

&#x20;             INTERNET




```

# ☁️ Cloudflare DNS and Tunnel

The DanSoftTech Infrastructure Lab uses Cloudflare DNS and Cloudflare

Tunnel to publish services hosted on the physical SERVER2025 environment.



The architecture allows public hostnames to be connected to services

running inside the laboratory infrastructure.



```



&#x20;                        INTERNET

&#x20;                           │

&#x20;                           ▼

&#x20;                      CLOUDFLARE

&#x20;                           │

&#x20;                    DNS / TUNNEL

&#x20;                           │

&#x20;                           ▼

&#x20;                 CLOUDFLARE TUNNEL

&#x20;                           │

&#x20;                           ▼

&#x20;                      CLOUDFLARED

&#x20;                           │

&#x20;                           ▼

&#x20;                     SERVER2025

&#x20;                           │

&#x20;                           ▼

&#x20;                      APACHE

&#x20;                           │

&#x20;                           ▼

&#x20;                      VIRTUALHOST

&#x20;                           │

&#x20;                           ▼

&#x20;                   C:\\xampp\\htdocs


```


\---



\# 🌍 Public IPv4 and Remote Access Validation



The DanSoftTech Infrastructure Lab was also validated through public

IPv4 connectivity provided by the ISP.



The public IPv4 environment was used to test real external access to

the laboratory infrastructure.



The validation included:



\- Internet connectivity

\- ISP equipment forwarding

\- MikroTik remote administration

\- SERVER2025 remote administration

\- WebFig access

\- WinBox access

\- Remote Desktop access



The public IPv4 address and administrative port numbers are intentionally

not exposed in this public repository.



Sensitive network information is maintained in the private laboratory

documentation.



\---



\## 🔐 Remote Administration Architecture



```

&#x20;                   INTERNET

&#x20;                      │

&#x20;                      ▼

&#x20;             PUBLIC IPv4 CONNECTION

&#x20;                      │

&#x20;                      ▼

&#x20;                ISP / HUAWEI

&#x20;                      │

&#x20;                      ▼

&#x20;                MIKROTIK RB2011

&#x20;                      │

&#x20;             ┌────────┴────────┐

&#x20;             │                 │

&#x20;             ▼                 ▼

&#x20;       SERVER2025          MANAGEMENT

&#x20;                               │

&#x20;                               ▼

&#x20;                          RYZEN 5X




```



# 🌐 Multi-Site Hosting



The DanSoftTech Infrastructure Lab was designed to host multiple

websites and services from the same physical SERVER2025 environment.



The multi-site architecture uses:



```

Cloudflare

&#x20;    │

&#x20;    ▼

Cloudflare Tunnel

&#x20;    │

&#x20;    ▼

SERVER2025

&#x20;    │

&#x20;    ▼

Apache

&#x20;    │

&#x20;    ▼

VirtualHosts

&#x20;    │

&#x20;    ├── Site / Service 01

&#x20;    ├── Site / Service 02

&#x20;    ├── Site / Service 03

&#x20;    ├── Support

&#x20;    ├── Forms

&#x20;    └── Other Applications

```



\# 🌐 Second Domain — criscerri.com.br



The DanSoftTech Infrastructure Lab also includes a second real domain

integrated into the hosting infrastructure.



The domain:



\*\*criscerri.com.br\*\*



is part of the real multi-site environment operated through the

DanSoftTech Infrastructure Lab.



The architecture extends the main DanSoftTech platform by connecting

the second domain to the same physical SERVER2025 environment.



```



DanSoftTech.com.br

&#x20;       │

&#x20;       ├── Cloudflare

&#x20;       ├── Cloudflare Tunnel

&#x20;       │

&#x20;       ▼

&#x20;    SERVER2025

&#x20;       │

&#x20;       ▼

&#x20;  Apache / XAMPP

&#x20;       │

&#x20;       ▼

&#x20;   VirtualHosts

&#x20;       │

&#x20;       ▼

&#x20;criscerri.com.br

&#x20;       │

&#x20;       ▼

&#x20;Cristiane Cerri

&#x20;Terapia Interativa



```



\---



\## 🔗 Real Domain Integration



The `criscerri.com.br` domain was integrated into the DanSoftTech

Infrastructure Lab as a real hosting service.



The integration connects the public domain to the physical

SERVER2025 environment through the following components:



```

criscerri.com.br

&#x20;       │

&#x20;       ▼

Cloudflare DNS

&#x20;       │

&#x20;       ▼

Cloudflare Tunnel

&#x20;       │

&#x20;       ▼

cloudflared

&#x20;       │

&#x20;       ▼

SERVER2025

&#x20;       │

&#x20;       ▼

Apache

&#x20;       │

&#x20;       ▼

VirtualHost

&#x20;       │

&#x20;       ▼

C:\\xampp\\htdocs



```


This architecture allows the public domain to reach a service hosted

inside the physical laboratory environment without exposing the

internal server directly to the public Internet.



The domain integration was implemented as part of the real

DanSoftTech hosting platform and tested through external access.



\---



\# 🔧 Real DNS and Apache Configuration



The second domain was integrated using real DNS and web server

configuration within the DanSoftTech Infrastructure Lab.



The project configuration files document the use of Cloudflare DNS,

Cloudflare Tunnel and Apache VirtualHosts for the `criscerri.com.br`

domain and its services.



\## Cloudflare DNS



The DanSoftTech automation scripts were created to manage DNS records

for the `criscerri.com.br` zone.



The documented process includes:



\- Identification of the `criscerri.com.br` DNS zone

\- Verification of existing CNAME records

\- Creation of CNAME records for subdomains

\- Association of the hostname with the Cloudflare Tunnel

\- Validation of the DNS configuration



The scripts are designed to avoid exposing Cloudflare credentials

inside the public documentation.



\## Apache VirtualHost



The Apache configuration includes a real VirtualHost for the main

`criscerri.com.br` domain.



```

criscerri.com.br

&#x20;       │

&#x20;       ▼

Apache VirtualHost

&#x20;       │

&#x20;       ▼

C:\\xampp\\htdocs\\criscerri

```



The documented Apache configuration uses:



```

ServerName criscerri.com.br

ServerAlias www.criscerri.com.br

DocumentRoot C:/xampp/htdocs/criscerri

```



The Apache configuration also defines access permissions and log

files for the hosted service.



\## Example Subdomain — agenda.criscerri.com.br



The project configuration also documents the `agenda` subdomain:



```

agenda.criscerri.com.br

&#x20;       │

&#x20;       ▼

Cloudflare / Tunnel

&#x20;       │

&#x20;       ▼

Apache

&#x20;       │

&#x20;       ▼

C:\\xampp\\htdocs\\agenda

```



The corresponding Apache VirtualHost uses:



```

ServerName agenda.criscerri.com.br

DocumentRoot C:/xampp/htdocs/agenda

```



This configuration demonstrates the real multi-site capability of the

laboratory, where different hostnames can be directed to different

applications hosted on the same physical SERVER2025 environment.



\---



\# 🧪 Technical Validation



The DanSoftTech Infrastructure Lab uses direct technical validation

before considering a service ready for operation.



The validation process includes the Cloudflare Tunnel configuration,

the Apache configuration and the Cloudflared service.



\## Cloudflare Tunnel Validation



The Tunnel configuration can be validated using:



```

cloudflared tunnel ingress validate

```



This command is used to validate the ingress configuration before

operational use.



\## Apache Configuration Validation



The Apache configuration can be validated using:



```

httpd.exe -t

```



This verifies the Apache configuration syntax before restarting or

reloading the web server.



\## Cloudflared Service Validation



The Windows service status can be checked using:



```

sc query Cloudflared

```



This allows the operational state of the Cloudflared service to be

verified directly on SERVER2025.



\## Validation Principle



The laboratory follows the principle:



```

CONFIGURATION

&#x20;     ↓

SYNTAX VALIDATION

&#x20;     ↓

SERVICE VALIDATION

&#x20;     ↓

EXTERNAL ACCESS TEST

&#x20;     ↓

DOCUMENTATION

```



The validation commands documented here are part of the real

operational procedures used in the DanSoftTech Infrastructure Lab.



\---



\# 🌍 External Access Validation



The DanSoftTech Infrastructure Lab was validated through real external

network access.



The validation was performed using the public IPv4 connectivity

provided by the ISP and the remote administration services configured

within the laboratory.



\## External Connectivity



The external validation included:



\- Internet connectivity

\- Public IPv4 reachability

\- ISP equipment forwarding

\- MikroTik remote administration

\- SERVER2025 remote administration

\- WebFig access

\- WinBox access

\- Remote Desktop access



The tests demonstrated that the laboratory infrastructure could be

accessed remotely through its configured network architecture.



\## Remote Administration



The remote administration architecture allows authorized management

of the laboratory infrastructure from an external network.



```

EXTERNAL NETWORK

&#x20;      │

&#x20;      ▼

PUBLIC IPv4

&#x20;      │

&#x20;      ▼

ISP / HUAWEI

&#x20;      │

&#x20;      ▼

MIKROTIK RB2011

&#x20;      │

&#x20;      ├── Remote Management

&#x20;      │

&#x20;      ▼

SERVER2025

&#x20;      │

&#x20;      └── Remote Desktop

```



The public IPv4 address and administrative port numbers are intentionally

omitted from this public documentation.



Sensitive network information remains restricted to the private

laboratory documentation.



\## Validation Scope



The external validation confirms the integration between the ISP

connection, MikroTik RouterOS, SERVER2025 and the remote administration

environment.



The laboratory documentation preserves the detailed network

configuration and evidence separately from this public repository.



\---



\# 📁 Evidence and Laboratory Records



The DanSoftTech Infrastructure Lab maintains technical evidence of

the infrastructure configuration, tests and operational environment.



The evidence is preserved separately from the public repository in

order to protect sensitive network information.



\## Real Evidence Records



The laboratory evidence includes technical screenshots, configuration

records, videos and documentation related to the physical infrastructure.



Examples of preserved evidence include:



```

PORTAS+IPV4.mp4

&#x20;       │

&#x20;       └── MikroTik remote access through IPv4



DNS+IPV4+CLOUDFLARED.mp4

&#x20;       │

&#x20;       └── DNS / IPv4 / Cloudflared demonstration



CATALOGO-DANSOFTECH.mp4

&#x20;       │

&#x20;       └── DanSoftTech infrastructure documentation

```



These records complement the technical documentation presented in this

repository and provide historical evidence of the laboratory evolution.



\## Evidence Preservation



The laboratory follows the principle:



```

REAL INFRASTRUCTURE

&#x20;       ↓

REAL TEST

&#x20;       ↓

REAL EVIDENCE

&#x20;       ↓

DOCUMENTATION

&#x20;       ↓

HISTORICAL PRESERVATION

```



Sensitive screenshots, IP addresses, administrative ports, credentials

and other private technical information are retained in the private

laboratory documentation and are not published in this repository.



The public documentation presents the architecture and technical

concepts while preserving the security of the operational environment.



\---



\# 📜 Infrastructure Evolution



The DanSoftTech Infrastructure Lab is the result of a continuous

evolution of a real physical technology environment.



The infrastructure was progressively developed, configured, tested

and expanded according to operational requirements.



The current laboratory represents the integration of networking,

server infrastructure, web hosting, remote administration and

Cloudflare services.



\## Evolution Path



```

Physical Infrastructure

&#x20;       ↓

SERVER2025

&#x20;       ↓

MikroTik RouterOS

&#x20;       ↓

Internet / IPv4 Connectivity

&#x20;       ↓

Remote Administration

&#x20;       ↓

Cloudflare DNS

&#x20;       ↓

Cloudflare Tunnel

&#x20;       ↓

Apache / XAMPP

&#x20;       ↓

VirtualHosts

&#x20;       ↓

Multi-Site Hosting

&#x20;       ↓

Second Domain

&#x20;       ↓

criscerri.com.br

&#x20;       ↓

DanSoftTech Infrastructure Lab

```



Each stage represents an expansion of the laboratory capabilities and

the integration of additional technologies into the physical

environment.



The infrastructure continues to serve as a real laboratory for

testing, validation, documentation and development.



\## Current Laboratory Concept



The DanSoftTech Infrastructure Lab is not a simulated environment.



It is a physical infrastructure where technologies are configured,

operated, tested and documented in real conditions.



The laboratory therefore serves both as an operational environment

and as a technical learning and validation platform.



\---



\# ✅ Final Validation Checklist



The DanSoftTech Infrastructure Lab maintains a final validation

checklist covering the main components of the physical environment.



\## Infrastructure Checklist



```

\[✓] Physical SERVER2025

\[✓] Windows Server 2025 Datacenter

\[✓] MikroTik RB2011

\[✓] ISP / Huawei connectivity

\[✓] Public / Fixed IPv4 connectivity

\[✓] Administrative network

\[✓] Management workstation

```



\## Hosting and Cloud Checklist



```

\[✓] Cloudflare DNS

\[✓] Cloudflare Tunnel

\[✓] cloudflared

\[✓] Apache / XAMPP

\[✓] VirtualHosts

\[✓] Multi-Site Hosting

\[✓] Second Domain — criscerri.com.br

\[✓] agenda.criscerri.com.br

```



\## Remote Administration Checklist



```

\[✓] External network access

\[✓] MikroTik remote administration

\[✓] WebFig

\[✓] WinBox

\[✓] SERVER2025 Remote Desktop

```



\## Validation Procedure Checklist



```

\[✓] Cloudflare Tunnel configuration validation

\[✓] Apache configuration syntax validation

\[✓] Cloudflared service verification

\[✓] External access validation

\[✓] Evidence preservation

\[✓] Technical documentation

```



\## Security and Documentation Checklist



```

\[✓] Public IPv4 protected from public documentation

\[✓] Administrative ports protected from public documentation

\[✓] Credentials excluded from public repository

\[✓] Private technical evidence maintained separately

\[✓] Real infrastructure documented

\[✓] Real tests documented

\[✓] Historical evidence preserved

```



\## Laboratory Validation Model



```

PHYSICAL INFRASTRUCTURE

&#x20;         ↓

NETWORK CONFIGURATION

&#x20;         ↓

SERVER CONFIGURATION

&#x20;         ↓

CLOUD SERVICES

&#x20;         ↓

WEB HOSTING

&#x20;         ↓

REMOTE ACCESS

&#x20;         ↓

TECHNICAL VALIDATION

&#x20;         ↓

REAL EVIDENCE

&#x20;         ↓

DOCUMENTATION

```



The checklist represents the infrastructure components and validation

procedures documented throughout this laboratory record.



Detailed sensitive configurations and private operational evidence

remain outside the public repository.



\---

