---
description: ''
layout: schema
name: LogContent
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: content
  type: string
- description: ''
  name: size
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-log-content-schema.json
slug: oracle-goldengate-rest-log-content
source_filename: oracle-goldengate-rest-log-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogContent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"content\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-log-content-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: LogContent
---
