---
description: ''
layout: schema
name: DatabaseStatistics
properties_list:
- description: ''
  name: processName
  type: string
- description: ''
  name: totalOperations
  type: integer
- description: ''
  name: inserts
  type: integer
- description: ''
  name: updates
  type: integer
- description: ''
  name: deletes
  type: integer
- description: ''
  name: truncates
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-database-statistics-schema.json
slug: oracle-goldengate-rest-database-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatabaseStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processName\": {\n      \"type\": \"string\"\n    },\n    \"totalOperations\": {\n      \"type\": \"integer\"\n    },\n    \"inserts\": {\n      \"type\": \"integer\"\n    },\n    \"updates\": {\n      \"type\": \"integer\"\n    },\n    \"deletes\": {\n      \"type\": \"integer\"\n    },\n    \"truncates\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-database-statistics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DatabaseStatistics
---
