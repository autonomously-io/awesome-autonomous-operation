# Awesome Prometheus 分析

> **Repository**: [roaldnefs/awesome-prometheus](https://github.com/roaldnefs/awesome-prometheus)

## 概要

Prometheus エコシステムに特化したリソース集。モニタリング・アラート・可視化のツールチェーン全体をカバー。

## 主要カテゴリ

| カテゴリ          | 内容                                                                |
| ----------------- | ------------------------------------------------------------------- |
| Tutorials         | Kubernetes 監視, Docker/CentOS セットアップ, Grafana 連携           |
| Deployment Tools  | Ansible roles, Kubernetes operators                                 |
| Exporters         | DB, ハードウェア, HTTP, その他システム向けデータコレクター          |
| Alertmanager      | アラート管理、ルーティング、重複排除                                |
| High Availability | Thanos, Cortex, VictoriaMetrics（長期ストレージ・スケーラビリティ） |
| Dashboards        | Grafana 連携                                                        |

## autonomously-io との関連性・優位性

Prometheus メトリクスは OpenObserve が直接取り込める形式。豊富な exporter エコシステムにより、追加の計装なしで既存インフラからメトリクス収集が可能。Alertmanager パターンは Keep のアラート管理と補完関係。
