---
description: ''
layout: schema
name: PipelineTarget
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: Target type
  name: type
  type: string
- description: ''
  name: connectionName
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-pipeline-target-schema.json
slug: oracle-goldengate-stream-analytics-rest-pipeline-target
source_filename: oracle-goldengate-stream-analytics-rest-pipeline-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PipelineTarget\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Target type\"\n    },\n    \"connectionName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-pipeline-target-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: PipelineTarget
---
