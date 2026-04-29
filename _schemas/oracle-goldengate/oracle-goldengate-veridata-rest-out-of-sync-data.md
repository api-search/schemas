---
description: ''
layout: schema
name: OutOfSyncData
properties_list:
- description: ''
  name: runId
  type: integer
- description: ''
  name: rows
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-out-of-sync-data-schema.json
slug: oracle-goldengate-veridata-rest-out-of-sync-data
source_filename: oracle-goldengate-veridata-rest-out-of-sync-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OutOfSyncData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"integer\"\n    },\n    \"rows\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-out-of-sync-data-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: OutOfSyncData
---
