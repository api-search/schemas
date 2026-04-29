---
description: ''
layout: schema
name: CreateTaskRequest
properties_list:
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
schema_file: json-schema/oracle-goldengate-rest-create-task-request-schema.json
slug: oracle-goldengate-rest-create-task-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTaskRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"type\": \"object\"\n    },\n    \"action\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-task-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateTaskRequest
---
