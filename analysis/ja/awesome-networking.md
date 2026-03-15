# Awesome Networking 分析

> **Repository**: [nyquist/awesome-networking](https://github.com/nyquist/awesome-networking) (624 stars)

## 概要

ネットワークの設計・実装・運用・監視をカバーするリソース集。ネットワークアーキテクチャからデイ2運用まで、ライフサイクル全体を網羅。

## 主要カテゴリ

| カテゴリ                | 内容                                              |
| ----------------------- | ------------------------------------------------- |
| Network Design          | Arista, Cisco, Cumulus, Juniper の設計ガイド      |
| Network Implementation  | ルーティング、スイッチング、VPN、シミュレータ     |
| Network Operations      | 変更管理、自動化、監視、インベントリ              |
| Monitoring Tools        | perfSONAR, LibreNMS, Observium, BGPAlerter        |
| Flow & Traffic Analysis | pmacct, Elastiflow, vFlow, goFlow, NexusFlowMeter |
| Performance Measurement | Vaping, UDPing, ToDD                              |

## 主要プロジェクト

- **perfSONAR** — フェデレーテッドネットワーク計測ツールキット
- **pmacct** — パッシブネットワーク監視（NetFlow, IPFIX, sFlow, BGP）
- **vFlow** — 高性能 IPFIX, sFlow, NetFlow コレクター
- **goFlow** — Cloudflare の NetFlow/IPFIX/sFlow コレクター
- **LibreNMS** — SNMP ベースの自動検出型監視
- **Zeek** — ネットワークセキュリティ監視フレームワーク

## autonomously-io との関連性・優位性

このリストは autonomously-io パイプラインにデータを供給するネットワーク監視・フロー分析のランドスケープを示す。Vector は sFlow/NetFlow/IPFIX データを取り込み、NATS がフローイベントを転送、OpenObserve が結果のテレメトリを保存・可視化。ここに挙げられたフロー収集ツールは、自律ネットワーク運用のデータソースとしての統合候補。
