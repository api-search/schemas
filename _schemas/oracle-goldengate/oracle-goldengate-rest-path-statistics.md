---
description: ''
layout: schema
name: PathStatistics
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: bytesProcessed
  type: integer
- description: ''
  name: messagesProcessed
  type: integer
- description: ''
  name: lag
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-path-statistics-schema.json
slug: oracle-goldengate-rest-path-statistics
source_filename: oracle-goldengate-rest-path-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PathStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"bytesProcessed\": {\n      \"type\": \"integer\"\n    },\n    \"messagesProcessed\": {\n      \"type\": \"integer\"\n    },\n    \"lag\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-path-statistics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: PathStatistics
---
