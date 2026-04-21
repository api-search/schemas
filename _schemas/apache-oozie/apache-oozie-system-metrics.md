---
description: Oozie server performance and operational metrics.
layout: schema
name: SystemMetrics
properties_list:
- description: Gauge metrics keyed by metric name.
  name: gauges
  type: object
- description: Counter metrics keyed by metric name.
  name: counters
  type: object
- description: Timer metrics keyed by metric name.
  name: timers
  type: object
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-system-metrics-schema.json
slug: apache-oozie-system-metrics
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: SystemMetrics
---
