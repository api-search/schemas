---
description: ''
layout: schema
name: HeartbeatMetrics
properties_list:
- description: ''
  name: processName
  type: string
- description: ''
  name: lastHeartbeat
  type: string
- description: ''
  name: lagInSeconds
  type: number
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-heartbeat-metrics-schema.json
slug: oracle-goldengate-rest-heartbeat-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HeartbeatMetrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processName\": {\n      \"type\": \"string\"\n    },\n    \"lastHeartbeat\": {\n      \"type\": \"string\"\n    },\n    \"lagInSeconds\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-heartbeat-metrics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: HeartbeatMetrics
---
