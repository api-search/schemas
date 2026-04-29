---
description: ''
layout: schema
name: Pipeline
properties_list:
- description: Pipeline unique identifier
  name: id
  type: string
- description: Pipeline display name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Current pipeline status
  name: status
  type: string
- description: ''
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: sources
  type: array
- description: ''
  name: targets
  type: array
- description: ''
  name: stages
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-pipeline-schema.json
slug: oracle-goldengate-stream-analytics-rest-pipeline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline unique identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline display name\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current pipeline status\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\"\n    },\n    \"sources\": {\n      \"type\": \"array\"\n    },\n    \"targets\": {\n      \"type\": \"array\"\n    },\n    \"stages\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-pipeline-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Pipeline
---
