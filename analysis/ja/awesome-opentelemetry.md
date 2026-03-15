# Awesome OpenTelemetry 分析

> **Repository**: [magsther/awesome-opentelemetry](https://github.com/magsther/awesome-opentelemetry)

## 概要

OpenTelemetry エコシステムに特化したリソース集。CNCF プロジェクトとしてベンダー非依存のテレメトリ標準を提供。

## 主要カテゴリ

| カテゴリ             | 内容                                                          |
| -------------------- | ------------------------------------------------------------- |
| Education            | 30 Days of OpenTelemetry コース                               |
| Books                | O'Reilly "The Future of Observability with OpenTelemetry" 等  |
| Distributed Tracing  | OSS（Jaeger, Zipkin, SigNoz）、ベンダー（Datadog, Dynatrace） |
| Client Libraries     | C++, .NET, Go, Java, JavaScript, Python, Ruby, Rust, Swift    |
| Collector Components | Receivers, Processors, Exporters                              |
| Storage Backends     | Cassandra, Elasticsearch, Tempo, Jaeger                       |

## autonomously-io との関連性・優位性

OpenTelemetry は Vector の入出力として直接対応しており、OTLP プロトコル経由で OpenObserve にデータを送信できる。標準化されたテレメトリ収集の基盤として、autonomously-io スタックとの親和性が高い。NATS も OTel コレクターと処理レイヤー間のトランスポートとして機能。
