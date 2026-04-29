---
description: ''
layout: schema
name: ProcessStatus
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lag
  type: string
- description: ''
  name: since
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-big-data-rest-process-status-schema.json
slug: oracle-goldengate-big-data-rest-process-status
source_filename: oracle-goldengate-big-data-rest-process-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lag\": {\n      \"type\": \"string\"\n    },\n    \"since\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-big-data-rest-process-status-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ProcessStatus
---
