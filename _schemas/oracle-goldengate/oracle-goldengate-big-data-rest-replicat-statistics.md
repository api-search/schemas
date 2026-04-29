---
description: ''
layout: schema
name: ReplicatStatistics
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
  name: handlerStatistics
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-big-data-rest-replicat-statistics-schema.json
slug: oracle-goldengate-big-data-rest-replicat-statistics
source_filename: oracle-goldengate-big-data-rest-replicat-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplicatStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"processName\": {\n      \"type\": \"string\"\n    },\n    \"totalOperations\": {\n      \"type\": \"integer\"\n    },\n    \"inserts\": {\n      \"type\": \"integer\"\n    },\n    \"updates\": {\n      \"type\": \"integer\"\n    },\n    \"deletes\": {\n      \"type\": \"integer\"\n    },\n    \"handlerStatistics\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-big-data-rest-replicat-statistics-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ReplicatStatistics
---
