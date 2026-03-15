# Awesome Observability - Analysis

> **Repository**: [adriannovegil/awesome-observability](https://github.com/adriannovegil/awesome-observability)

## Overview

Comprehensive resource collection covering the "three pillars" of observability (metrics, logs, distributed traces) across the entire pipeline from collection to visualization.

## Main Categories

| Category            | Description                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------- |
| Collect             | Metrics (OpenTelemetry, Prometheus exporters), Tracing (Sleuth, inspectIT), Logging (Elastic Beats) |
| Transport           | Kafka, NATS, RabbitMQ, Redis                                                                        |
| Collectors          | Prometheus, Telegraf, Graylog, Loki                                                                 |
| Storage             | TSDB (InfluxDB, VictoriaMetrics), Tracing (Zipkin, Jaeger, Tempo), Search (Elasticsearch)           |
| Visualization       | Grafana, tracing UIs, uptime monitoring                                                             |
| Processing & Alerts | Logstash, Fluentd, Vector                                                                           |
| Load Generators     | JMeter, K6, Locust, Gatling                                                                         |
| APM Solutions       | Application performance monitoring platforms                                                        |
| Service Mesh        | Distributed system observability                                                                    |

## Relevance & Advantages for autonomously-io

The autonomously-io stack (OpenObserve + Vector + NATS) maps to the Storage + Processing + Transport layers in this list. OpenObserve replaces the traditional Elasticsearch + Grafana combination, while Vector unifies the collection/processing layer. This list is useful for evaluating alternative and complementary components.
