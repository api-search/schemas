---
description: ''
layout: schema
name: Replicat
properties_list:
- description: Replicat process name
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: Source trail file
  name: trail
  type: string
- description: Big data handler type
  name: handler
  type: string
- description: Parameter file content including handler configuration
  name: config
  type: array
- description: Path to handler properties file
  name: handlerProperties
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-big-data-rest-replicat-schema.json
slug: oracle-goldengate-big-data-rest-replicat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Replicat\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Replicat process name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Source trail file\"\n    },\n    \"handler\": {\n      \"type\": \"string\",\n      \"description\": \"Big data handler type\"\n    },\n    \"config\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter file content including handler configuration\"\n    },\n    \"handlerProperties\": {\n      \"type\": \"string\",\n      \"description\": \"Path to handler properties file\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-big-data-rest-replicat-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Replicat
---
