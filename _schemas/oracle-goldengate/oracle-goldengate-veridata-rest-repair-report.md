---
description: ''
layout: schema
name: RepairReport
properties_list:
- description: ''
  name: runId
  type: integer
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: totalRows
  type: integer
- description: ''
  name: repairedRows
  type: integer
- description: ''
  name: failedRows
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-repair-report-schema.json
slug: oracle-goldengate-veridata-rest-repair-report
source_filename: oracle-goldengate-veridata-rest-repair-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"integer\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"totalRows\": {\n      \"type\": \"integer\"\n    },\n    \"repairedRows\": {\n      \"type\": \"integer\"\n    },\n    \"failedRows\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-repair-report-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: RepairReport
---
