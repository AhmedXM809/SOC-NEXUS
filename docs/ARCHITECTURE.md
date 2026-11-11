# SOC NEXUS - Architecture Overview

## Project Purpose
SOC NEXUS is a centralized Security Operations and Automation Center.

## Core Technologies
| Technology | Responsibility |
|---|---|
| Splunk Enterprise | Security monitoring and detection visibility |
| n8n | Workflow automation |
| MISP | Threat intelligence and IOC enrichment |
| TheHive | Incident and case management |

## Logical Architecture

`mermaid
flowchart TB
    Analyst[ SOC Analyst ] --> Nexus[ SOC NEXUS ]
    Nexus --- Splunk[ Splunk Enterprise ]
    Nexus --- N8N[ n8n Automation ]
    Nexus --- MISP[ Threat Intelligence ]
    Nexus --- Hive[ TheHive ]
`",
    ",

- Centralized security operations overview.
- System health monitoring.
- Detection analytics and incident exploration.
- Investigation and evidence visibility.
- Automation history and response visibility.
- Secure analyst access.
- Configurable audio notifications.

## Security
Project descriptions identify HTTPS, password hashing, CSRF protection, and secure sessions.
These controls have not been independently audited through this showcase.

## Deployment Scope
The original application remains on Debian.
This repository currently contains documentation and visual assets, not application source code.
The architecture above is logical and does not claim verified API connections or network topology.
