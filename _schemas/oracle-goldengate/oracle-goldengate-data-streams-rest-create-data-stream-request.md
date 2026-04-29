---
description: ''
layout: schema
name: CreateDataStreamRequest
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: source
  type: object
- description: ''
  name: target
  type: object
- description: ''
  name: filters
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-data-streams-rest-create-data-stream-request-schema.json
slug: oracle-goldengate-data-streams-rest-create-data-stream-request
source_filename: oracle-goldengate-data-streams-rest-create-data-stream-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDataStreamRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"object\"\n    },\n    \"target\": {\n      \"type\": \"object\"\n    },\n    \"filters\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-data-streams-rest-create-data-stream-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateDataStreamRequest
---
