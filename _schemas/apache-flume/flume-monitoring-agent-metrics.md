---
description: All component metrics for a Flume agent indexed by component type and name
layout: schema
name: AgentMetrics
properties_list: []
provider_name: Apache Flume
provider_slug: apache-flume
schema_file: json-schema/flume-monitoring-agent-metrics-schema.json
slug: flume-monitoring-agent-metrics
source_filename: flume-monitoring-agent-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flume/refs/heads/main/json-schema/flume-monitoring-agent-metrics-schema.json\",\n  \"title\": \"AgentMetrics\",\n  \"description\": \"All component metrics for a Flume agent indexed by component type and name\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/ComponentMetrics\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flume/refs/heads/main/json-schema/flume-monitoring-agent-metrics-schema.json
tags:
- Apache
- Data Collection
- ETL
- Log Aggregation
- Open Source
- Streaming
title: AgentMetrics
---
