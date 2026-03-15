# Awesome 5G 分析

> **Repository**: [calee0219/awesome-5g](https://github.com/calee0219/awesome-5g)

## 概要

5G スタック全体の OSS 実装集。プロトコルライブラリとテストツールが充実。

## 主要カテゴリ

| カテゴリ          | 内容                                                |
| ----------------- | --------------------------------------------------- |
| SIM               | SIM/UICC カード管理・設定ツール                     |
| UE/CPE            | ユーザー端末、CPE                                   |
| RAN               | 無線アクセスネットワークスタック・シミュレータ      |
| Core Network      | 5G コア実装（free5GC, Open5GS, OAI-CN）             |
| Platforms         | オーケストレーション・管理・デプロイ（Magma, ONAP） |
| NFs               | ネットワーク機能実装（UPF, ゲートウェイ）           |
| Edge/Applications | MEC, ネットワークスライシング, IoT                  |
| Protocols         | GTP, SCTP, NGAP, PFCP, Diameter, NAS ライブラリ     |
| Tools             | テスト、可視化、仕様検索                            |
| Research          | 学術・実験プロジェクト                              |

## 主要プロジェクト

- **free5GC / Open5GS / OAI-CN** — オープンソース 5G コアネットワーク
- **UERANSIM / srsRAN / free5GRAN** — RAN ソリューション
- **Magma / ONAP** — オーケストレーションプラットフォーム
- **5G Trace Visualizer** — pcap からのコールフロー可視化

## autonomously-io との関連性・優位性

自律運用の対象環境を提供。プロトコルライブラリ（GTP, PFCP 等）とトレースツールは、Vector が 5G インフラから収集するテレメトリの理解に不可欠。テストツール・シミュレータにより自律運用ワークフローの検証が可能。
