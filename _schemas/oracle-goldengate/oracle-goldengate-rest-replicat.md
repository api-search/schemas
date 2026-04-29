---
description: ''
layout: schema
name: Replicat
properties_list:
- description: Replicat process name
  name: name
  type: string
- description: Type of replicat
  name: type
  type: string
- description: Current process status
  name: status
  type: string
- description: ''
  name: description
  type: string
- description: Source trail file path
  name: trail
  type: string
- description: Checkpoint table name
  name: checkpointTable
  type: string
- description: Parameter file content lines
  name: config
  type: array
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-replicat-schema.json
slug: oracle-goldengate-rest-replicat
source_filename: oracle-goldengate-rest-replicat-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Replicat\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Replicat process name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of replicat\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current process status\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Source trail file path\"\n    },\n    \"checkpointTable\": {\n      \"type\": \"string\",\n      \"description\": \"Checkpoint table name\"\n    },\n    \"config\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter file content lines\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-replicat-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Replicat
---
