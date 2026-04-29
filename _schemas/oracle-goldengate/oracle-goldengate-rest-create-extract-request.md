---
description: ''
layout: schema
name: CreateExtractRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: Begin position (NOW, SCN value, or timestamp)
  name: begin
  type: string
- description: Trail file prefix (e.g., aa)
  name: trail
  type: string
- description: Trail file size in MB (default 500)
  name: trailSize
  type: integer
- description: Parameter file content
  name: config
  type: array
- description: ''
  name: registration
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-extract-request-schema.json
slug: oracle-goldengate-rest-create-extract-request
source_filename: oracle-goldengate-rest-create-extract-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateExtractRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"begin\": {\n      \"type\": \"string\",\n      \"description\": \"Begin position (NOW, SCN value, or timestamp)\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Trail file prefix (e.g., aa)\"\n    },\n    \"trailSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Trail file size in MB (default 500)\"\n    },\n    \"config\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter file content\"\n    },\n    \"registration\": {\n      \"type\": \"string\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-extract-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateExtractRequest
---
