---
description: ''
layout: schema
name: ProcessMetrics
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lag
  type: number
- description: ''
  name: checkpointLag
  type: number
- description: ''
  name: inputBytes
  type: integer
- description: ''
  name: outputBytes
  type: integer
- description: ''
  name: operationsProcessed
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-process-metrics-schema.json
slug: oracle-goldengate-rest-process-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessMetrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lag\": {\n      \"type\": \"number\"\n    },\n    \"checkpointLag\": {\n      \"type\": \"number\"\n    },\n    \"inputBytes\": {\n      \"type\": \"integer\"\n    },\n    \"outputBytes\": {\n      \"type\": \"integer\"\n    },\n    \"operationsProcessed\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-process-metrics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ProcessMetrics
---
