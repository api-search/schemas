---
description: ''
layout: schema
name: DataStream
properties_list:
- description: Unique data stream name
  name: name
  type: string
- description: Stream description
  name: description
  type: string
- description: Current stream status
  name: status
  type: string
- description: Source configuration
  name: source
  type: object
- description: Target distribution configuration
  name: target
  type: object
- description: Table and operation filters
  name: filters
  type: array
- description: Path to the AsyncAPI specification
  name: asyncApiSpec
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-data-streams-rest-data-stream-schema.json
slug: oracle-goldengate-data-streams-rest-data-stream
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataStream\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique data stream name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Stream description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current stream status\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"Source configuration\"\n    },\n    \"target\": {\n      \"type\": \"object\",\n      \"description\": \"Target distribution configuration\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"Table and operation filters\"\n    },\n    \"asyncApiSpec\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the AsyncAPI specification\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"\
  updatedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-data-streams-rest-data-stream-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DataStream
---
