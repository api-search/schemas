---
description: ''
layout: schema
name: HeartbeatTable
properties_list:
- description: Schema owner of the heartbeat table
  name: owner
  type: string
- description: Heartbeat table name
  name: table
  type: string
- description: Retention time in days
  name: retentionTime
  type: integer
- description: Update frequency in seconds
  name: frequency
  type: integer
- description: Purge frequency in minutes
  name: purgeFrequency
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-heartbeat-table-schema.json
slug: oracle-goldengate-rest-heartbeat-table
source_filename: oracle-goldengate-rest-heartbeat-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HeartbeatTable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Schema owner of the heartbeat table\"\n    },\n    \"table\": {\n      \"type\": \"string\",\n      \"description\": \"Heartbeat table name\"\n    },\n    \"retentionTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Retention time in days\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Update frequency in seconds\"\n    },\n    \"purgeFrequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Purge frequency in minutes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-heartbeat-table-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: HeartbeatTable
---
