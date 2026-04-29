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
source_filename: apache-oozie-system-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-system-metrics-schema.json\",\n  \"title\": \"SystemMetrics\",\n  \"description\": \"Oozie server performance and operational metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gauges\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Gauge metrics keyed by metric name.\"\n    },\n    \"counters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Counter metrics keyed by metric name.\"\n    },\n    \"timers\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Timer metrics keyed by metric name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-system-metrics-schema.json
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
