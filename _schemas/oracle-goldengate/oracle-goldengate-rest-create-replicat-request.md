---
description: ''
layout: schema
name: CreateReplicatRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: Source trail file prefix
  name: trail
  type: string
- description: Checkpoint table in format schema.table
  name: checkpointTable
  type: string
- description: ''
  name: begin
  type: string
- description: Parameter file content
  name: config
  type: array
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-replicat-request-schema.json
slug: oracle-goldengate-rest-create-replicat-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateReplicatRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Source trail file prefix\"\n    },\n    \"checkpointTable\": {\n      \"type\": \"string\",\n      \"description\": \"Checkpoint table in format schema.table\"\n    },\n    \"begin\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter file content\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-replicat-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateReplicatRequest
---
