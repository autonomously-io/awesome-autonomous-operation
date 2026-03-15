# Awesome Telco 分析

> **Repository**: [ravens/awesome-telco](https://github.com/ravens/awesome-telco)

## 概要

SIM カードから 5G コア、RAN、セキュリティ、ラボ環境まで、モバイルネットワークスタック全体をカバーする OSS カタログ。

## 主要カテゴリ

| カテゴリ             | 内容                                            |
| -------------------- | ----------------------------------------------- |
| SIM Cards            | PySIM, sysmoISIM, eSIM/eUICC 管理               |
| User Equipment       | 4G/5G モデム、診断ツール（QCSuper, SCAT）       |
| Radio Access Network | O-RAN, 5G gNodeB, 4G eNodeB, PHY レイヤーツール |
| Core Network         | 5GC（Open5GS, free5GC, OAI）、EPC, UPF          |
| Interconnect         | IMS, SBC, SS7, Diameter                         |
| Infrastructure       | NFV, SDN, Kubernetes デプロイ                   |
| Orchestration        | 自動化・デプロイツール                          |
| Lab & Testbeds       | テスト環境                                      |
| Security             | セキュリティリサーチ、脆弱性分析                |

## 主要プロジェクト

- **Open5GS** — オープンソース 5G コア
- **free5GC** — 5GC 実装（Go）
- **UERANSIM** — 5G UE/RAN シミュレータ
- **srsRAN** — ソフトウェア無線 RAN

## autonomously-io との関連性・優位性

テレコムネットワークは RAN・Core・Transport から膨大なテレメトリを生成。Vector で収集、OpenObserve で分析・可視化、Keep で自動対応を統合し、テレコム自律運用の基盤を形成。
