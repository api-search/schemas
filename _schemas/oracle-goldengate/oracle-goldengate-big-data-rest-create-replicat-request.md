---
description: ''
layout: schema
name: CreateReplicatRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: trail
  type: string
- description: ''
  name: begin
  type: string
- description: ''
  name: config
  type: array
- description: ''
  name: checkpointTable
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-big-data-rest-create-replicat-request-schema.json
slug: oracle-goldengate-big-data-rest-create-replicat-request
source_filename: oracle-goldengate-big-data-rest-create-replicat-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateReplicatRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"trail\": {\n      \"type\": \"string\"\n    },\n    \"begin\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"array\"\n    },\n    \"checkpointTable\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-big-data-rest-create-replicat-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateReplicatRequest
---
