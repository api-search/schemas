---
description: ''
layout: schema
name: DataStreamSummary
properties_list:
- description: Data stream name
  name: name
  type: string
- description: Stream status
  name: status
  type: string
- description: Source trail or extract
  name: source
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-data-streams-rest-data-stream-summary-schema.json
slug: oracle-goldengate-data-streams-rest-data-stream-summary
source_filename: oracle-goldengate-data-streams-rest-data-stream-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataStreamSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data stream name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Stream status\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source trail or extract\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-data-streams-rest-data-stream-summary-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DataStreamSummary
---
