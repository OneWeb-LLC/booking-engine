# Managed Network Infrastructure

Status: **Reference architecture / planned Snapshot component.**

The Booking Engine depends on more than CRM software. If the network is unreliable, calls, notifications, SIP endpoints, tablets, workstations, and staff handoffs become unreliable.

## Doctrine

Networking belongs to the **Hardware & Channels** layer of the Booking Engine.

A network upgrade is justified only when it materially improves the Booking Engine's ability to create and sustain conversations, appointments, handoffs, or measurable revenue operations.

Do not replace a functioning client network solely to sell hardware.

## Default certification

- **Professional default:** Ubiquiti UniFi
- **Value alternative:** TP-Link Omada
- **Security-heavy:** Fortinet
- **Enterprise:** Cisco Meraki / HPE Aruba as requirements justify
- **Existing/temporary:** Google/Nest Wi-Fi may remain in place for simple pilots that do not need advanced management

## Why UniFi is the default

For the target SMB deployment, UniFi offers a strong balance of:
- gateway/firewall management
- managed switching and PoE
- business Wi-Fi
- VLANs
- guest isolation
- QoS / voice prioritization
- multi-site remote administration
- no mandatory recurring license for core management

## Standard logical design

Use only the segmentation that the client actually needs.

Typical managed deployment:
- Business network
- Voice network
- IoT network
- Guest network

A dedicated Voice VLAN and QoS become the preferred design once phone volume, device count, support requirements, or call-quality risk justify the additional complexity.

## Communications relationship

The current GHI phone pilot may run on the existing Google mesh first. The objective is to prove SIP calling, Yealink endpoints/headsets, CRM/Booking Engine continuity, and employee execution before changing the underlying network.

After the communications workflow is proven, a UniFi reference deployment can be dogfooded at GHI and converted into a sellable Salesflow Telecom managed-network package.

## Commercial packages

- OneWeb Network Essential — value managed network
- OneWeb Network Professional — default UniFi managed infrastructure
- OneWeb Network Secure — deeper security/compliance
- OneWeb Network Enterprise — enterprise-selected architecture

## Completion evidence for a supported Snapshot component

Before this moves from reference architecture to supported Booking Engine Snapshot:
- reference BOM
- configuration template
- VLAN/QoS policy
- remote support procedure
- backup/restore procedure
- install checklist
- phone call-quality verification
- failure/rollback procedure
- client handoff/training procedure
- unit economics and support burden from at least one real deployment

Execution is backlog-gated behind ONE-12 where autonomous implementation or merge/release work is involved.
