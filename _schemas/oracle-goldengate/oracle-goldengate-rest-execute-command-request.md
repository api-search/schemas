---
description: ''
layout: schema
name: ExecuteCommandRequest
properties_list:
- description: GGSCI command to execute (e.g., INFO ALL, STATUS EXTRACT *)
  name: command
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-execute-command-request-schema.json
slug: oracle-goldengate-rest-execute-command-request
source_filename: oracle-goldengate-rest-execute-command-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteCommandRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"command\": {\n      \"type\": \"string\",\n      \"description\": \"GGSCI command to execute (e.g., INFO ALL, STATUS EXTRACT *)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-execute-command-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ExecuteCommandRequest
---
