# Awesome 5G - Analysis

> **Repository**: [calee0219/awesome-5g](https://github.com/calee0219/awesome-5g)

## Overview

Curated collection of open-source implementations across the complete 5G stack, from radio access through core networks to edge applications. Strong emphasis on protocol libraries and testing tools.

## Main Categories

| Category          | Description                                         |
| ----------------- | --------------------------------------------------- |
| SIM               | SIM/UICC card management and configuration tools    |
| UE/CPE            | User equipment and customer premises equipment      |
| RAN               | Radio access network stacks and simulators          |
| Core Network      | 5G core implementations (free5GC, Open5GS, OAI-CN)  |
| Platforms         | Orchestration, management, deployment (Magma, ONAP) |
| NFs               | Network function implementations (UPF, gateways)    |
| Edge/Applications | MEC, network slicing, IoT                           |
| Protocols         | GTP, SCTP, NGAP, PFCP, Diameter, NAS libraries      |
| Tools             | Testing, visualization, specification lookup        |
| Research          | Academic and experimental projects                  |

## Key Projects

- **free5GC / Open5GS / OAI-CN** — Open source 5G core networks
- **UERANSIM / srsRAN / free5GRAN** — RAN solutions
- **Magma / ONAP** — Orchestration platforms
- **5G Trace Visualizer** — Call flow visualization from pcap

## Relevance & Advantages for autonomously-io

Provides the target environment for autonomous operations. The protocol libraries (GTP, PFCP, etc.) and trace tools are essential for understanding the telemetry that Vector collects from 5G infrastructure. The test tools and simulators enable validation of autonomous operation workflows.
