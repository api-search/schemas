---
description: ''
layout: schema
name: CollectorPath
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: Target trail file
  name: trail
  type: string
- description: ''
  name: port
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-collector-path-schema.json
slug: oracle-goldengate-rest-collector-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectorPath\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"trail\": {\n      \"type\": \"string\",\n      \"description\": \"Target trail file\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-collector-path-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CollectorPath
---
