---
description: ''
layout: schema
name: ProcessCommand
properties_list:
- description: Command action to execute
  name: action
  type: string
- description: Additional command options
  name: options
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-process-command-schema.json
slug: oracle-goldengate-rest-process-command
source_filename: oracle-goldengate-rest-process-command-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessCommand\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Command action to execute\"\n    },\n    \"options\": {\n      \"type\": \"string\",\n      \"description\": \"Additional command options\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-process-command-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ProcessCommand
---
