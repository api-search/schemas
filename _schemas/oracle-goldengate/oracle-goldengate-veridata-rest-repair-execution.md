---
description: ''
layout: schema
name: RepairExecution
properties_list:
- description: ''
  name: runId
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: startTime
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-repair-execution-schema.json
slug: oracle-goldengate-veridata-rest-repair-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairExecution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-repair-execution-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: RepairExecution
---
