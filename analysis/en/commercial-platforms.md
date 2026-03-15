# Commercial Autonomous Operation Platforms - Analysis

## Platform Comparison

| Platform            | Key Strength                                                                                                    | TMF AN Level     | Real Deployments                                |
| ------------------- | --------------------------------------------------------------------------------------------------------------- | ---------------- | ----------------------------------------------- |
| **Google ANO**      | GNN + Digital Twin (Spanner Graph), zero-copy data architecture (70% storage reduction)                         | -                | One NZ, Deutsche Telekom, Vodafone, Telstra     |
| **Microsoft NOA**   | Azure NetAI track record (60% faster fault detection), policy-gated governance                                  | -                | Far EasTone, Vodafone                           |
| **Nokia AVA**       | Deepest telecom domain expertise, eBPF-based observability, cross-domain (IP/optical/wireless/core) correlation | -                | Deutsche Telekom                                |
| **Cisco Crosswork** | Federated data access (Cisco/customer/3rd party), Toxic Factor Identification                                   | -                | Beta phase                                      |
| **Ericsson NWDAF**  | Only 3GPP-standardized analytics function, 45% OPEX/CAPEX reduction                                             | **L4 certified** | TDC NET (world's first L4), DNB Malaysia        |
| **Huawei ADN**      | 4-domain coverage (wireless/core/optical/IP), most production deployments                                       | **L4**           | China Mobile (multiple provinces), AIS Thailand |
| **HPE Mist AI**     | Experience-centric (LEM), graduated autonomy model, natural language troubleshooting                            | -                | Aberdeen City Council, airports                 |
| **NVIDIA AI-RAN**   | RAN + AI dynamic allocation on same GPU (2-3x utilization), Apache 2.0 open-source                              | -                | T-Mobile US 2026 trial                          |

## 6 Capabilities Commercial Has That OSS Lacks

### 1. Telecom Domain Models

Commercial platforms (Nokia's telco-trained LLM/LAM/ML, Huawei's Telecom Foundation Model, NVIDIA's Nemotron LTM, Google's GNN models) are trained on massive proprietary telecom datasets — alarm correlations, topology patterns, fault signatures from hundreds of operator networks. Open-source stacks have the plumbing but no pre-trained telecom intelligence.

### 2. Network Digital Twins

Google (Spanner Graph + GNN), Nokia (AVA), Huawei (ADN), and HPE (Marvis Minis + Apstra graph DB) maintain live digital twins of network topology, state, and behavior. This enables predictive operations — detecting problems before they manifest. OpenObserve stores telemetry but does not model topology or relationships.

### 3. Cross-Domain Closed-Loop Automation

Commercial platforms implement closed loops spanning multiple network domains (RAN, transport, core, IT) with built-in safety guardrails, rollback mechanisms, and graduated autonomy. Keep operates within a single domain and lacks cross-domain orchestration, conflict resolution, and safety envelopes.

### 4. Governance, Audit, and Trust Frameworks

Microsoft NOA's policy-gated actions, HPE Marvis's graduated autonomy controls, and Cisco's approval workflows reflect years of enterprise trust-building. No open-source stack has built-in concepts of "this agent can auto-remediate Wi-Fi AP reboots but requires human approval for routing changes."

### 5. Vendor Ecosystem Integration

Commercial platforms have pre-built integrations with hundreds of network element types, NMS systems, OSS/BSS stacks, and domain-specific protocols (NETCONF/YANG models, 3GPP interfaces, O-RAN E2 interfaces). Open-source relies on generic protocols (SNMP, syslog, OpenTelemetry) and requires custom integration per vendor.

### 6. TMF AN Level Certification

Multiple commercial vendors (Ericsson/TDC NET, Huawei/China Mobile) have achieved certified TMF Level 4 autonomy. No open-source stack has been assessed against any TMF AN Level. The evaluation methodology itself (ANLET/IG1252) assumes capabilities that do not exist in open-source tooling today.

## What OSS Does Better

- **Cost structure** — No per-node or per-agent licensing
- **Transparency** — No black-box AI
- **Data sovereignty** — No telemetry leaving the operator's infrastructure
- **Composability** — Multi-cloud/on-prem deployment flexibility
- **Evolution speed** — Keep, OpenObserve, Vector all ship weekly

## TMF Autonomous Network Levels (L0-L5)

| Level | Name        | Description                                                         |
| ----- | ----------- | ------------------------------------------------------------------- |
| L0    | Manual      | All manual, no scripting                                            |
| L1    | Assisted    | Tool-assisted but all decisions by humans                           |
| L2    | Partial     | Specific task automation, human monitors and approves               |
| L3    | Conditional | Conditional autonomy within defined scope, humans handle exceptions |
| L4    | High        | High autonomy with closed-loop operations, humans monitor only      |
| L5    | Full        | Full autonomy, zero-touch, no human intervention required           |

## Sources

- [Google Cloud ANO Framework](https://cloud.google.com/blog/topics/telecommunications/the-autonomous-network-operations-framework-for-csps)
- [Microsoft NOA Introduction](https://techcommunity.microsoft.com/blog/telecommunications-industry-blog/introducing-microsoft%E2%80%99s-network-operations-agent-%E2%80%93-a-telco-framework-for-autonom/4471185)
- [Nokia AVA Platform](https://www.nokia.com/ai-and-analytics/ai-for-network-efficiency/)
- [Cisco Crosswork Multi-Agentic AI](https://www.cisco.com/c/en/us/products/collateral/networking/software/crosswork-network-automation/crosswork-multi-agentic-ai-framework-aag.html)
- [Ericsson NWDAF](https://www.ericsson.com/en/core-network/5g-core/network-data-analytics-function)
- [Ericsson/TDC NET L4 Certification](https://www.ericsson.com/en/news/2025/6/tdc-net-and-ericsson-achieves-industry-first-certification-from-tm-forum-of-level-4-autonomy)
- [Huawei ADN](https://carrier.huawei.com/en/adn)
- [HPE Mist Agentic AI](https://www.hpe.com/us/en/newsroom/press-release/2025/08/hpe-accelerates-self-driving-network-operations-with-new-mist-agentic-ai-native-innovations.html)
- [NVIDIA AI Aerial](https://developer.nvidia.com/industries/telecommunications/ai-aerial)
- [TMF Autonomous Networks](https://www.tmforum.org/missions/autonomous-networks)
- [TMF AN Levels Evaluation IG1252](https://www.tmforum.org/resources/introductory-guide/ig1252-autonomous-network-levels-evaluation-methodology-v1-2-0/)
