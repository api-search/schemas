---
description: ''
layout: schema
name: ComparisonReport
properties_list:
- description: ''
  name: runId
  type: integer
- description: ''
  name: jobName
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: summary
  type: object
- description: ''
  name: details
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-comparison-report-schema.json
slug: oracle-goldengate-veridata-rest-comparison-report
source_filename: oracle-goldengate-veridata-rest-comparison-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComparisonReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"integer\"\n    },\n    \"jobName\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"type\": \"object\"\n    },\n    \"details\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-comparison-report-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ComparisonReport
---
