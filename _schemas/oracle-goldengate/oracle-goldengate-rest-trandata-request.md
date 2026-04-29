---
description: ''
layout: schema
name: TrandataRequest
properties_list:
- description: ''
  name: operation
  type: string
- description: Table or schema name
  name: name
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-trandata-request-schema.json
slug: oracle-goldengate-rest-trandata-request
source_filename: oracle-goldengate-rest-trandata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TrandataRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Table or schema name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-trandata-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: TrandataRequest
---
