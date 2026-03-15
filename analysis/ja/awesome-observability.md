# Awesome Observability 分析

> **Repository**: [adriannovegil/awesome-observability](https://github.com/adriannovegil/awesome-observability)

## 概要

Observability の「三本柱」（メトリクス・ログ・分散トレース）を軸に、収集から可視化までのパイプライン全体を網羅したリソース集。

## 主要カテゴリ

| カテゴリ            | 内容                                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------------------- |
| Collect             | メトリクス（OpenTelemetry, Prometheus exporters）、トレース（Sleuth, inspectIT）、ログ（Elastic Beats） |
| Transport           | Kafka, NATS, RabbitMQ, Redis                                                                            |
| Collectors          | Prometheus, Telegraf, Graylog, Loki                                                                     |
| Storage             | TSDB（InfluxDB, VictoriaMetrics）、トレース（Zipkin, Jaeger, Tempo）、検索（Elasticsearch）             |
| Visualization       | Grafana, トレース UI, アップタイム監視                                                                  |
| Processing & Alerts | Logstash, Fluentd, Vector                                                                               |
| Load Generators     | JMeter, K6, Locust, Gatling                                                                             |
| APM Solutions       | アプリケーションパフォーマンス監視                                                                      |
| Service Mesh        | 分散システムのオブザーバビリティ                                                                        |

## autonomously-io との関連性・優位性

autonomously-io スタック（OpenObserve + Vector + NATS）はこのリストの Storage + Processing + Transport レイヤーに対応。OpenObserve が従来の Elasticsearch + Grafana を、Vector が収集・処理レイヤーを統合。代替・補完コンポーネントの評価に有用。
