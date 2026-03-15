<p align="center">
  <img src="assets/logo-banner.svg" alt="Awesome Autonomous Operation" width="100%">
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
</p>

A curated list of awesome resources for AI-driven autonomous operations — a concept encompassing observability, telecom automation, AIOps, and beyond.

## Contents

- [Similar Projects & Awesome Lists](#similar-projects--awesome-lists)
- [Autonomous Operation Platforms](#autonomous-operation-platforms)
- [Observability](#observability)
- [Data Pipeline](#data-pipeline)
- [AIOps](#aiops)
- [Telecom Automation](#telecom-automation)
- [Self-Healing & Auto-Remediation](#self-healing--auto-remediation)
- [LLM/AI for Operations](#llmai-for-operations)
- [Incident Management & SRE](#incident-management--sre)
- [Network Monitoring & Flow Analysis](#network-monitoring--flow-analysis)
- [Related Papers & Standards](#related-papers--standards)

---

## Similar Projects & Awesome Lists

- [Awesome AIOps](https://github.com/linjinjin123/awesome-AIOps) - Curated list of AIOps resources including papers, tools, and datasets. → [Analysis](analysis/en/awesome-aiops.md)
- [Awesome Observability](https://github.com/adriannovegil/awesome-observability) - Curated list of observability tools, frameworks, and resources. → [Analysis](analysis/en/awesome-observability.md)
- [Awesome Site Reliability Engineering](https://github.com/dastergon/awesome-sre) - Curated list of SRE resources. → [Analysis](analysis/en/awesome-sre.md)
- [Awesome Network Automation](https://github.com/networktocode/awesome-network-automation) - Curated list of network automation resources. → [Analysis](analysis/en/awesome-network-automation.md)
- [Awesome Telco](https://github.com/ravens/awesome-telco) - Curated list of telecom resources. → [Analysis](analysis/en/awesome-telco.md)
- [Awesome 5G](https://github.com/calee0219/awesome-5g) - Curated list of 5G projects and resources. → [Analysis](analysis/en/awesome-5g.md)
- [Awesome Telco Cloud](https://github.com/LesFacilitateurs/awesome-telco-cloud) - Curated list of Telco Cloud ecosystem projects. → [Analysis](analysis/en/awesome-telco-cloud.md)
- [Awesome Self-Hosting](https://github.com/awesome-selfhosted/awesome-selfhosted) - Self-hosted services and applications. → [Analysis](analysis/en/awesome-selfhosted.md)
- [Awesome Prometheus](https://github.com/roaldnefs/awesome-prometheus) - Curated list of Prometheus resources. → [Analysis](analysis/en/awesome-prometheus.md)
- [Awesome OpenTelemetry](https://github.com/magsther/awesome-opentelemetry) - Curated list of OpenTelemetry resources. → [Analysis](analysis/en/awesome-opentelemetry.md)
- [Awesome Sysadmin](https://github.com/awesome-foss/awesome-sysadmin) - Curated list of open-source sysadmin resources. Comprehensive monitoring, log management, and metrics sections.
- [Awesome SNMP](https://github.com/eozer/awesome-snmp) - Curated list of SNMP resources — libraries, CLI tools, GUIs, MIB repositories, and RFCs.
- [Awesome Monitoring](https://github.com/crazy-canux/awesome-monitoring) - Infrastructure, OS, and application monitoring tools.
- [Awesome Incident Management](https://github.com/JupiterOne/awesome-incident-management) - Curated list of incident management resources.

## Autonomous Operation Platforms

### Open Source

- [ONAP](https://www.onap.org/) ([GitHub](https://github.com/ONAP)) - Open Network Automation Platform for real-time, policy-driven orchestration and automation.
  - Full MANO + closed-loop automation. The most complete open source telecom automation platform.
- [Nephio](https://nephio.org/) ([GitHub](https://github.com/nephio-project)) - Cloud native intent automation for telecom.
  - Kubernetes-native. Uses KRM (Kubernetes Resource Model) for intent-based NF deployment.
- [StackStorm](https://github.com/StackStorm/st2) - Event-driven automation platform for auto-remediation and ChatOps.
  - If-this-then-that automation with 160+ integrations. Bridges IT and network operations.
- [Rundeck](https://github.com/rundeck/rundeck) - Operations automation with runbook management.
- [OSM (Open Source MANO)](https://osm.etsi.org/) - ETSI-hosted NFV Management and Orchestration stack.

### Commercial / Industry Solutions

- [Google Cloud Autonomous Network Operations](https://cloud.google.com/blog/topics/telecommunications/the-autonomous-network-operations-framework-for-csps) - Blueprint for CSPs transitioning from manual to zero-touch operations.
  - [New Agents for ANO](https://cloud.google.com/blog/topics/telecommunications/new-agents-for-the-autonomous-network-operations-framework) - Autonomous Data Steward and VoLTE Agents with agentic AI.
  - [GraphML and Digital Twins](https://cloud.google.com/blog/topics/telecommunications/graphml-and-digital-twins-enable-autonomous-networks) - Graph Neural Networks for predictive network management.
- [Microsoft Network Operations Agent (NOA)](https://techcommunity.microsoft.com/blog/telecommunications-industry-blog/introducing-microsoft%E2%80%99s-network-operations-agent-%E2%80%93-a-telco-framework-for-autonom/4471185) - Multi-agent framework for autonomous network operations.
  - [NOA Framework Evolution](https://techcommunity.microsoft.com/blog/telecommunications-industry-blog/evolving-the-network-operations-agent-framework-driving-the-next-wave-of-autonom/4496607) - Specialized agents for NOC, ticketing, telemetry.
  - [Microsoft NetAI](https://techcommunity.microsoft.com/blog/telecommunications-industry-blog/reimagining-network-operations-how-microsoft-netai-tackles-hyperscale-challenges/4470572) - Internal AI achieving 60% faster fault detection on Azure network.
- [Nokia AVA Platform](https://www.nokia.com/networks/technologies/ava-cognitive-services-platform/) - AI and analytics platform for cognitive network operations.
  - [Autonomous Operations Vision](https://www.nokia.com/blog/autonomous-operations-is-it-time-for-a-new-network-operating-system/) - Proposes unified operations layer spanning network and IT.
- [Cisco Crosswork](https://www.cisco.com/site/us/en/products/networking/software/crosswork-network-automation/index.html) - Intent-based, closed-loop network automation suite.
  - [Multi-Agentic AI Framework](https://www.cisco.com/c/en/us/products/collateral/networking/software/crosswork-network-automation/crosswork-multi-agentic-ai-framework-aag.html) - Specialized AI agents coordinated by a meta-agent.
  - [Agentic NOC Operations](https://www.cisco.com/c/en/us/products/collateral/cloud-systems-management/crosswork-network-automation/c11-5510101-00-optimizing-noc-operations-through-an-agentic-approach-wp-v1a.html) - Vision for NOCless/Dark NOC operations.
- [Ericsson NWDAF](https://www.ericsson.com/en/core-network/5g-core/network-data-analytics-function) - 3GPP-standardized Network Data Analytics Function for 5G core.
- [Huawei ADN](https://carrier.huawei.com/en/adn) - Autonomous Driving Network with GenAI, agents, and digital twins.
  - [Campus L4 ADN (MWC 2026)](https://www.huawei.com/en/news/2026/3/mwc-l4-autonomous-driving) - Industry's first L4 autonomous network deployment.
- [HPE Mist AI](https://www.hpe.com/us/en/mist-ai.html) - AI-native networking for self-driving networks.
  - [Mist Agentic AI](https://www.hpe.com/us/en/newsroom/press-release/2025/08/hpe-accelerates-self-driving-network-operations-with-new-mist-agentic-ai-native-innovations.html) - Marvis AI agents for cross-domain autonomous remediation.
- [NVIDIA Telecom AI](https://www.nvidia.com/en-us/industries/telecommunications/ai/) - GPU-accelerated AI for telecom.
  - [AI Aerial](https://developer.nvidia.com/industries/telecommunications/ai-aerial) - Accelerated computing platform for AI-native wireless networks.
  - [AI-RAN](https://www.nvidia.com/en-us/industries/telecommunications/ai-ran/) - Converges AI workloads and RAN processing on shared GPU infrastructure.

## Observability

- [OpenObserve](https://github.com/openobserve/openobserve) - Petabyte scale Elasticsearch/Splunk/Datadog alternative for logs, metrics, traces, RUM, errors, and session replay. ⭐ _autonomously-io component_
- [Keep](https://github.com/keephq/keep) - Open source AIOps and alert management platform with AI correlation and YAML workflow automation. ⭐ _autonomously-io component_
- [Prometheus](https://github.com/prometheus/prometheus) - Monitoring system and time series database.
- [Grafana](https://github.com/grafana/grafana) - Open and composable observability and data visualization platform.
- [Jaeger](https://github.com/jaegertracing/jaeger) - Distributed tracing platform.
- [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-collector) - Vendor-agnostic telemetry data collection. The universal observability data plane.
- [SigNoz](https://github.com/SigNoz/signoz) - Open-source APM and observability platform. OpenTelemetry-native.
- [Graylog](https://github.com/Graylog2/graylog2-server) - Log management platform.

## Data Pipeline

- [Vector](https://github.com/vectordotdev/vector) - High-performance observability data pipeline. ⭐ _autonomously-io component_
- [NATS](https://github.com/nats-io/nats-server) - High-performance cloud-native messaging system. ⭐ _autonomously-io component_
- [Fluentd](https://github.com/fluent/fluentd) - Unified logging layer.
- [Fluent Bit](https://github.com/fluent/fluent-bit) - Lightweight log processor and forwarder.
- [Apache Kafka](https://github.com/apache/kafka) - Distributed event streaming platform.
- [Logstash](https://github.com/elastic/logstash) - Server-side data processing pipeline.

## AIOps

### Open Source

- [PyRCA](https://github.com/salesforce/PyRCA) - Python ML library for metric-based root cause analysis (Salesforce).
  - Implements Bayesian, PC, GES, and causal discovery methods for RCA.
- [LogAI](https://github.com/salesforce/logai) - Open source library for AI-based log analytics (Salesforce).
  - Log summarization, clustering, anomaly detection, and pattern mining.
- [Qdrant](https://github.com/qdrant/qdrant) - Vector similarity search engine for RAG-based operational knowledge retrieval. ⭐ _autonomously-io component_

### Commercial

- [Moogsoft](https://www.moogsoft.com/) - AI-powered IT operations platform. Pioneered AIOps category.
- [BigPanda](https://www.bigpanda.io/) - Event correlation and automation for IT operations. Open Box ML for explainable correlation.
- [Dynatrace](https://www.dynatrace.com/) - Software intelligence platform with Davis AI engine.
- [Datadog](https://www.datadoghq.com/product/network-monitoring/) - Unified IT and network monitoring.

## Telecom Automation

### Open Source 5G Core

- [free5GC](https://free5gc.org/) ([GitHub](https://github.com/free5gc/free5gc)) - Open source 5G core network based on 3GPP R15+ (Go).
- [Open5GS](https://open5gs.org/open5gs/docs/) ([GitHub](https://github.com/open5gs/open5gs)) - C-language 5G Core and EPC implementation (Release-17).
- [OpenAirInterface](https://openairinterface.org/) - Open source 4G/5G RAN and Core from EURECOM.
- [SD-Core (Aether)](https://docs.sd-core.aetherproject.org/) ([GitHub](https://github.com/omec-project)) - Disaggregated 4G/5G mobile core for cloud and edge.

### Open Source RAN

- [srsRAN Project](https://www.srsran.com/) ([GitHub](https://github.com/srsran/srsRAN_Project)) - O-RAN native 5G CU/DU in portable C++.
- [srsRAN 4G](https://github.com/srsran/srsRAN_4G) - Open source SDR 4G software suite (eNB, UE, EPC).
- [O-RAN SC](https://o-ran-sc.org/) - O-RAN Software Community for open RAN automation.

### Platforms & Infrastructure

- [Anuket](https://anuket.io/) - Common reference infrastructure for telecom.
- [LF Networking](https://lfnetworking.org/) - Umbrella for open source networking projects (ONAP, FD.io, Nephio, etc.).
- [Duranta (LFN + OAI)](https://www.linuxfoundation.org/press/lf-networking-and-openairinterface-software-alliance-osa-collaborate-to-announce-duranta-to-advance-open-source-ran-innovation) - Joint LFN/OAI initiative for open source RAN.
- [OPNFV](https://www.opnfv.org/) - Open platform for NFV.
- [XOS / CORD](https://opennetworking.org/cord/) - Central Office Re-architected as a Datacenter.

## Self-Healing & Auto-Remediation

- [Kuberhealthy](https://github.com/kuberhealthy/kuberhealthy) - Kubernetes operator for synthetic monitoring and auto-healing.
- [Chaos Mesh](https://github.com/chaos-mesh/chaos-mesh) - Cloud-native chaos engineering platform.
- [Litmus](https://github.com/litmuschaos/litmus) - Chaos engineering framework for Kubernetes.
- [Keptn](https://github.com/keptn/keptn) - Cloud-native application life-cycle orchestration with automated quality gates.
- [Crossplane](https://github.com/crossplane/crossplane) - Cloud-native control plane for infrastructure. Extends Kubernetes to manage any resource.

## LLM/AI for Operations

### Frameworks & Models

- [TelecomGPT](https://arxiv.org/abs/2407.09424) - Framework to build telecom-specific LLMs. Fine-tuned Llama3-8B outperforms GPT-4 on telecom tasks.
- [NetLLM (SIGCOMM 2024)](https://dl.acm.org/doi/10.1145/3651890.3672268) - First framework adapting LLMs for networking tasks (viewport prediction, ABR, scheduling).
- [MeshAgent (SIGMETRICS 2026)](https://zaoxing.github.io/papers/2026/SIGMETRICS26_MeshAgent.pdf) - LLM agent for reliable network management using constraint-based knowledge extraction.
- [MM-Telco](https://arxiv.org/html/2511.13131v1) - Multimodal LLM benchmarks for telecom applications.
- [Network Arena](https://arxiv.org/html/2512.16381v1) - Benchmark arena for evaluating AI agents on network troubleshooting.
- [GSMA Open-Telco LLM Benchmarks](https://www.gsma.com/get-involved/gsma-foundry/gsma-open-telco-llm-benchmarks/) ([Hugging Face](https://huggingface.co/otellm)) - Open-source benchmark evaluating AI models on telecom use cases.

### Surveys

- [LLM for Telecom Survey](https://arxiv.org/abs/2405.10825) - Comprehensive survey on LLM principles, techniques, and opportunities in telecom.
- [LLM-Based Network Management Survey](https://onlinelibrary.wiley.com/doi/abs/10.1002/nem.70029) - Survey on LLM-based network management and operations (2025).
- [AIOps in the Era of LLMs](https://dl.acm.org/doi/10.1145/3746635) - Survey of 183 papers (2020-2024) on LLMs in AIOps.
- [LLMs for Telecom Standards](https://arxiv.org/html/2404.02929v1) - RAG-based approach to make 3GPP/ETSI specifications accessible via natural language.

## Incident Management & SRE

### Incident Management

- [PagerDuty](https://www.pagerduty.com/) - Digital operations management with AI-powered incident response.
- [Rootly](https://rootly.com/) - Incident management with Slack-native workflows and automated runbooks.
- [incident.io](https://incident.io/) - Incident management built for modern engineering teams.
- [Backstage](https://github.com/backstage/backstage) - CNCF developer portal for service catalog and operational tooling.

### SRE Practices

- [Google SRE Books](https://sre.google/books/) - Foundational texts on Site Reliability Engineering.
  - SLO/SLI/SLA frameworks, error budgets, and toil reduction — directly applicable to network operations.
- [OpenSLO](https://github.com/OpenSLO/OpenSLO) - Open specification for defining SLOs as code. Applicable to both IT services and network KPIs.
- [Sloth](https://github.com/slok/sloth) - SLO generation for Prometheus.

### Infrastructure as Code

- [Kubernetes](https://kubernetes.io/) - Container orchestration. The convergence point for telecom CNFs and IT workloads.
- [Terraform](https://www.terraform.io/) - IaC for multi-cloud and on-premises. Providers exist for network devices and cloud infrastructure.
- [Ansible Network Automation](https://www.ansible.com/use-cases/network-automation) - Agentless automation for network and IT infrastructure.
- [YANG Models Repository](https://github.com/YangModels/yang) - Community repository of YANG data models for model-driven network management.

## Network Monitoring & Flow Analysis

### Awesome Lists

- [Awesome Networking](https://github.com/nyquist/awesome-networking) - Curated list of networking resources including monitoring, automation, and design. → [Analysis](analysis/en/awesome-networking.md)
- [Awesome Sysadmin - Monitoring](https://github.com/kahun/awesome-sysadmin#monitoring) - Monitoring section of the awesome sysadmin list.

### Infrastructure Monitoring

- [Zabbix](https://github.com/zabbix/zabbix) - Enterprise-class open source monitoring for networks, servers, and applications. SNMP, IPMI, JMX, agent-based.
- [LibreNMS](https://github.com/librenms/librenms) - Auto-discovering network monitoring with SNMP support, alerting, and device tracking.
- [Nagios](https://github.com/NagiosEnterprises/nagioscore) - Industry-standard infrastructure monitoring. Extensive plugin ecosystem.
- [Icinga](https://github.com/Icinga/icinga2) - Scalable monitoring system, fork of Nagios with modern architecture.
- [Cacti](https://github.com/Cacti/cacti) - Network graphing solution using SNMP and RRDtool.
- [Observium](https://www.observium.org/) - Low-maintenance auto-discovering network monitoring with SNMP.
- [Checkmk](https://github.com/Checkmk/checkmk) - Infrastructure and application monitoring with auto-discovery.
- [Netdata](https://github.com/netdata/netdata) - Real-time full-stack monitoring with per-second metrics and zero-config agent. 78k stars.
- [OpenNMS](https://github.com/OpenNMS/opennms) - Enterprise-grade network management platform. SNMP, flow analysis, topology discovery.
- [NetBox](https://github.com/netbox-community/netbox) - The premier source of truth for network infrastructure. IPAM, DCIM, and network documentation. 20k stars.

### Flow Collection & Analysis (sFlow / NetFlow / IPFIX)

- [ntopng](https://github.com/ntop/ntopng) - Web-based traffic and security network monitoring. sFlow, NetFlow, IPFIX support. 7.6k stars.
- [Akvorado](https://github.com/akvorado/akvorado) - Flow collector, enricher, and visualizer. sFlow, NetFlow, IPFIX with ClickHouse backend.
- [goflow2](https://github.com/netsampler/goflow2) - High-performance sFlow/IPFIX/NetFlow collector. Successor to Cloudflare's goflow.
- [pmacct](https://github.com/pmacct/pmacct) - Passive network monitoring tools. NetFlow, IPFIX, sFlow, and BGP collection.
- [Elastiflow](https://github.com/robcowart/elastiflow) - Network flow analytics (NetFlow, sFlow, IPFIX) with the Elastic Stack.
- [FastNetMon](https://github.com/pavel-odintsov/fastnetmon) - High-speed DDoS detection via sFlow, NetFlow, IPFIX, and port mirroring.
- [vFlow](https://github.com/Edgio/vflow) - Enterprise network flow collector (IPFIX, sFlow, NetFlow).
- [nfdump](https://github.com/phaag/nfdump) - NetFlow/sFlow/IPFIX processing tools.
- [flow-pipeline](https://github.com/cloudflare/flow-pipeline) - Tools and examples for operating sFlow and NetFlow pipelines (Cloudflare).

### Active Measurement & Probing

- [perfSONAR](https://www.perfsonar.net/) ([GitHub](https://github.com/perfsonar), [Docs](https://docs.perfsonar.net/intro_about.html)) - Federated network measurement toolkit (OWAMP, TWAMP, iperf3, traceroute).
- [SmokePing](https://oss.oetiker.ch/smokeping/) ([GitHub](https://github.com/oetiker/SmokePing)) - Latency measurement with RRDtool graphing and pattern-based alerting.
- [Vaping](https://github.com/20c/vaping) - Healthy alternative to SmokePing — pluggable latency and reachability testing.
- [UDPing](https://github.com/yahoo/UDPing) - Measures latency and packet loss using UDP.

### TWAMP / STAMP

- [RFC 5357 - TWAMP](https://datatracker.ietf.org/doc/html/rfc5357) - Two-Way Active Measurement Protocol.
- [RFC 8762 - STAMP](https://datatracker.ietf.org/doc/html/rfc8762) - Simple Two-Way Active Measurement Protocol.
- [RFC 8972 - STAMP Extensions](https://datatracker.ietf.org/doc/rfc8972/) - Optional extensions for STAMP performance metrics.
- [RFC 9503 - STAMP for SR](https://www.rfc-editor.org/rfc/rfc9503.html) - STAMP extensions for Segment Routing (SR-MPLS and SRv6).
- [TWAMP Overview (Juniper)](https://www.juniper.net/documentation/us/en/software/junos/flow-monitoring/topics/concept/twamp-overview.html) - Two-Way Active Measurement Protocol implementation overview.
- [twampy](https://github.com/gcotone/twampy) - Python tools for TWAMP and TWAMP Light (STAMP).
- [twamp-rs](https://github.com/thatdevsherry/twamp-rs) - TWAMP (RFC 5357) implementation in Rust.
- [twamp (Go)](https://github.com/snormore/twamp) - Minimal TWAMP Light (RFC 5357) implementation in Go.
- [twamp_exporter](https://github.com/shmuto/twamp_exporter) - Prometheus exporter for bi-directional network latency measurement via TWAMP.
- [vMark](https://github.com/xmas-ar/vMark) - Carrier Ethernet demarcation management system with TWAMP support.

### Packet Capture & Deep Analysis

- [Arkime](https://github.com/arkime/arkime) - Large-scale full packet capture, indexing, and database system.
- [Zeek](https://github.com/zeek/zeek) - Powerful network analysis framework for security monitoring.
- [Sniffnet](https://github.com/GyulyVGC/sniffnet) - Cross-platform network traffic monitor with real-time visualization. 33k stars.
- [Suricata](https://github.com/OISF/suricata) - Network intrusion detection/prevention engine with protocol analysis.

## Related Papers & Standards

### Standards & Frameworks

- [TMF Autonomous Networks](https://www.tmforum.org/missions/autonomous-networks) - TM Forum's autonomous networks initiative and maturity levels (L0-L5).
  - [AN Levels (ANL) Model](https://www.tmforum.org/learn/education/autonomous-network-levels-anl-model/) - Classification from L0 (manual) to L5 (fully autonomous).
  - [AN Technical Architecture](https://www.tmforum.org/resources/toolkit/autonomous-networks-technical-architecture/) - Technical architecture toolkit.
  - [AN Levels Evaluation IG1252](https://www.tmforum.org/resources/introductory-guide/ig1252-autonomous-network-levels-evaluation-methodology-v1-2-0/) - Evaluation methodology.
- [ETSI ZSM](https://www.etsi.org/technologies/zero-touch-network-service-management) - Zero-touch network & Service Management.
  - [ZSM Closed-Loop Enablers](https://www.etsi.org/newsroom/blogs/technologies/entry/the-recently-released-etsi-zsm-specification-on-closed-loop-enablers-provides-a-significant-boost-for-enabling-full-end-to-end-network-and-service-automation) - OODA loop pattern for network automation.
  - [GR ZSM 011 - Intent-Driven Closed-Loop](https://zsmwiki.etsi.org/index.php?title=Topic_3_-_Intent-driven_Closed-Loop_automation) - Intent as key enabler for autonomous management.
  - [GR ZSM 011 v2.1.1 (PDF)](https://www.etsi.org/deliver/etsi_gr/ZSM/001_099/011/02.01.01_60/gr_ZSM011v020101p.pdf) - Full intent-driven AN specification.
- [ETSI ENI](https://www.etsi.org/technologies/experiential-networked-intelligence) - Experiential Networked Intelligence using AI for network management.
- [ETSI White Paper No. 40 (PDF)](https://www.etsi.org/images/files/ETSIWhitePapers/etsi-wp-40-Autonomous-networks.pdf) - Autonomous networks supporting tomorrow's ICT. Addresses telecom-IT convergence.
- [3GPP SON](https://www.3gpp.org/technologies/son) - Self-Organizing Networks: self-configuration, self-optimization, self-healing.
- [ITU-T Y.3172](https://www.itu.int/rec/T-REC-Y.3172) - Architectural framework of machine learning in future networks.
- [ITU-T Y.3060 - AN Trust](https://www.itu.int/epublications/publication/itu-t-y-3060-2023-09-autonomous-networks-overview-on-trust) - Trust principles (accountability, explainability, safety) in autonomous networks.
- [ITU-T Y.3061 - AN Architecture](https://www.itu.int/epublications/publication/itu-t-y-3061-2023-12-autonomous-networks-architecture-framework) - Architecture framework with Autonomy Engine.
- [O-RAN Alliance](https://www.o-ran.org/about) - Open, intelligent, virtualized, interoperable mobile networks.
- [GSMA AI for Networks](https://www.gsma.com/solutions-and-impact/technologies/artificial-intelligence/ai-for-networks/) - Industry-wide AI/ML program for network operations.
  - [GSMA Agentic AI in Telecom](https://www.gsma.com/solutions-and-impact/technologies/artificial-intelligence/agentic-ai-telecom/) - Multi-agent architectures for autonomous networks.

### Academic Papers

- [AI for 5G/6G Survey (MDPI 2025)](https://www.mdpi.com/2227-7080/13/12/559) - Taxonomy of AI applications, trends, and challenges in 5G/6G.
- [ZSM for 5G and Beyond Survey](https://www.sciencedirect.com/science/article/pii/S1084804522000297) - Comprehensive survey on ZSM architecture and implementation.
- [AI-Driven ZSM in 5G (IEEE)](https://ieeexplore.ieee.org/document/8994961/) - Challenges: data quality, model interpretability, safety constraints.
- [ML for O-RAN Automation (MDPI)](https://www.mdpi.com/1424-8220/23/21/8792) - ML applications for RIC-based RAN optimization.
- [Open-Source 5G Core Evaluation](https://arxiv.org/abs/2412.21162) - Performance comparison of Open5GS, free5GC, and OpenAirInterface.
- [TelecomGPT (IEEE)](https://ieeexplore.ieee.org/document/11097898/) - Framework to build telecom-specific LLMs with novel benchmarks.
- [Network Standardization (ITU)](https://www.itu.int/en/ITU-T/academia/kaleidoscope/2020/Documents/Network_Control_and_Management_Automation_Architecture_Standardization_Perspective.pdf) - Network automation architecture standardization perspective.

---

> ⭐ = [autonomously-io](https://github.com/autonomously-io) program component

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.
