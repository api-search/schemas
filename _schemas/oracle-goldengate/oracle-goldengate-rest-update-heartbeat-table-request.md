---
description: ''
layout: schema
name: UpdateHeartbeatTableRequest
properties_list:
- description: ''
  name: retentionTime
  type: integer
- description: ''
  name: frequency
  type: integer
- description: ''
  name: purgeFrequency
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-update-heartbeat-table-request-schema.json
slug: oracle-goldengate-rest-update-heartbeat-table-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateHeartbeatTableRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"retentionTime\": {\n      \"type\": \"integer\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\"\n    },\n    \"purgeFrequency\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-update-heartbeat-table-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: UpdateHeartbeatTableRequest
---
