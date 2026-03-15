# 商用自律運用プラットフォーム分析

## プラットフォーム比較

| プラットフォーム    | 最大の強み                                                                             | TMF AN Level | 実デプロイ                                  |
| ------------------- | -------------------------------------------------------------------------------------- | ------------ | ------------------------------------------- |
| **Google ANO**      | GNN + Digital Twin（Spanner Graph）、ゼロコピーデータアーキテクチャで70%ストレージ削減 | -            | One NZ, Deutsche Telekom, Vodafone, Telstra |
| **Microsoft NOA**   | Azure NetAI の実績（60%高速障害検知）、ポリシーゲート付きガバナンス                    | -            | Far EasTone, Vodafone                       |
| **Nokia AVA**       | 最深のテレコムドメイン知識、eBPF ベース監視、クロスドメイン（IP/光/無線/コア）相関     | -            | Deutsche Telekom                            |
| **Cisco Crosswork** | フェデレーテッドデータアクセス（Cisco/顧客/3rd party）、Toxic Factor Identification    | -            | Beta段階                                    |
| **Ericsson NWDAF**  | 唯一の3GPP標準準拠、45% OPEX/CAPEX削減                                                 | **L4認定**   | TDC NET（世界初L4）, DNB Malaysia           |
| **Huawei ADN**      | 4ドメイン横断（無線/コア/光/IP）、最も多い実デプロイ                                   | **L4**       | China Mobile 複数省, AIS Thailand           |
| **HPE Mist AI**     | ユーザー体験起点（LEM）、段階的自律化モデル、自然言語トラブルシュート                  | -            | Aberdeen City Council, 空港等               |
| **NVIDIA AI-RAN**   | RAN+AI を同一GPUで動的配分（2-3x利用率）、Apache 2.0 OSS化                             | -            | T-Mobile US 2026トライアル                  |

## 商用が持ち、OSS に無い6つの機能

### 1. テレコムドメインモデル

商用プラットフォーム（Nokia のテレコム専用 LLM/LAM/ML、Huawei の Telecom Foundation Model、NVIDIA の Nemotron LTM、Google の GNN モデル）は、数百のオペレータネットワークから収集した膨大な独自データセット（アラーム相関、トポロジパターン、障害シグネチャ）で学習済み。OSS スタックにはパイプラインはあるが、学習済みテレコムインテリジェンスがない。

### 2. Network Digital Twin

Google（Spanner Graph + GNN）、Nokia（AVA）、Huawei（ADN）、HPE（Marvis Minis + Apstra グラフ DB）は、ネットワークトポロジ・状態・振る舞いのライブ Digital Twin を維持。問題が発現する前に検知する予測運用を実現。OpenObserve はテレメトリ保存のみで、トポロジやリレーションのモデリングはない。

### 3. クロスドメイン Closed-Loop 自動化

商用プラットフォームは複数ネットワークドメイン（RAN、トランスポート、コア、IT）を横断するクローズドループを実装。安全ガードレール、ロールバック機構、段階的自律化を内蔵。Keep は単一ドメイン内で動作し、クロスドメインオーケストレーション、競合解決、安全エンベロープが不足。

### 4. ガバナンス・監査・信頼フレームワーク

Microsoft NOA のポリシーゲート付きアクション、HPE Marvis の段階的自律化コントロール、Cisco の承認ワークフロー。OSS スタックには「このエージェントは Wi-Fi AP 再起動を自動復旧できるが、ルーティング変更は人間の承認が必要」という概念がない。

### 5. ベンダーエコシステム統合

商用プラットフォームは数百の NE タイプ、NMS、OSS/BSS、ドメイン固有プロトコル（NETCONF/YANG、3GPP インターフェース、O-RAN E2）へのプリビルトコネクタを保有。OSS は汎用プロトコル（SNMP、syslog、OpenTelemetry）に依存し、ベンダー毎にカスタム統合が必要。

### 6. TMF AN Level 認定

Ericsson/TDC NET、Huawei/China Mobile が TMF Level 4 自律化を認定取得済み。OSS スタックで TMF AN Level の評価を受けたものはない。

## OSS の優位性

- **コスト構造** — ノード/エージェント課金なし
- **透明性** — ブラックボックス AI ではない
- **データ主権** — テレメトリが外部に出ない
- **組み合わせの自由度** — マルチクラウド/オンプレ
- **進化速度** — Keep, OpenObserve, Vector は毎週リリース

## TMF Autonomous Network Levels（L0-L5）

| Level | 名称        | 内容                                                 |
| ----- | ----------- | ---------------------------------------------------- |
| L0    | Manual      | 全て人手。スクリプトもなし                           |
| L1    | Assisted    | ツール支援あるが判断は全て人間                       |
| L2    | Partial     | 特定タスクの自動化。人間が監視・承認                 |
| L3    | Conditional | 条件付き自律。特定スコープ内で自動判断、例外は人間   |
| L4    | High        | 高度自律。クローズドループで自動運用、人間は監視のみ |
| L5    | Full        | 完全自律。ゼロタッチ、人間介入不要                   |

## autonomously-io が IT 向けに提供する価値

商用テレコムプラットフォームの機能を IT 領域に OSS で同等提供する。TMF AN Level フレームワークを IT 運用の成熟度指標として援用し、「IT 自律運用基盤として L3 相当」といった位置づけが可能。

## 出典

- [Google Cloud ANO Framework](https://cloud.google.com/blog/topics/telecommunications/the-autonomous-network-operations-framework-for-csps)
- [Microsoft NOA Introduction](https://techcommunity.microsoft.com/blog/telecommunications-industry-blog/introducing-microsoft%E2%80%99s-network-operations-agent-%E2%80%93-a-telco-framework-for-autonom/4471185)
- [Nokia AVA Platform](https://www.nokia.com/ai-and-analytics/ai-for-network-efficiency/)
- [Cisco Crosswork Multi-Agentic AI](https://www.cisco.com/c/en/us/products/collateral/networking/software/crosswork-network-automation/crosswork-multi-agentic-ai-framework-aag.html)
- [Ericsson NWDAF](https://www.ericsson.com/en/core-network/5g-core/network-data-analytics-function)
- [Ericsson/TDC NET L4 認定](https://www.ericsson.com/en/news/2025/6/tdc-net-and-ericsson-achieves-industry-first-certification-from-tm-forum-of-level-4-autonomy)
- [Huawei ADN](https://carrier.huawei.com/en/adn)
- [HPE Mist Agentic AI](https://www.hpe.com/us/en/newsroom/press-release/2025/08/hpe-accelerates-self-driving-network-operations-with-new-mist-agentic-ai-native-innovations.html)
- [NVIDIA AI Aerial](https://developer.nvidia.com/industries/telecommunications/ai-aerial)
- [TMF Autonomous Networks](https://www.tmforum.org/missions/autonomous-networks)
- [TMF AN Levels 評価メソドロジ IG1252](https://www.tmforum.org/resources/introductory-guide/ig1252-autonomous-network-levels-evaluation-methodology-v1-2-0/)
