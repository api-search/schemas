---
description: ''
layout: schema
name: Task
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: schedule
  type: object
- description: ''
  name: action
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-task-schema.json
slug: oracle-goldengate-rest-task
source_filename: oracle-goldengate-rest-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"type\": \"object\"\n    },\n    \"action\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-task-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Task
---
