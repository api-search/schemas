---
description: ''
layout: schema
name: Extract
properties_list:
- description: Extract process name
  name: name
  type: string
- description: Type of extract
  name: type
  type: string
- description: Current process status
  name: status
  type: string
- description: ''
  name: description
  type: string
- description: Begin position (NOW, SCN value, or timestamp)
  name: begin
  type: string
- description: Trail file path
  name: trail
  type: string
- description: Trail file size in MB
  name: trailSize
  type: integer
- description: Parameter file content lines
  name: config
  type: array
- description: Database registration alias
  name: registration
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-extract-schema.json
slug: oracle-goldengate-rest-extract
source_filename: oracle-goldengate-rest-extract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Extract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Extract process name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of extract\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current process status\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"begin\": {\n      \"type\": \"string\",\n      \"description\": \"Begin position (NOW, SCN value, or timestamp)\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Trail file path\"\n    },\n    \"trailSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Trail file size in MB\"\n    },\n    \"config\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter file content lines\"\n    },\n    \"registration\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Database registration alias\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-extract-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Extract
---
