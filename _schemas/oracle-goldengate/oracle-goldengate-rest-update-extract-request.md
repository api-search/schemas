---
description: ''
layout: schema
name: UpdateExtractRequest
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: config
  type: array
- description: ''
  name: credentials
  type: object
- description: ''
  name: begin
  type: string
- description: ''
  name: status
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-update-extract-request-schema.json
slug: oracle-goldengate-rest-update-extract-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateExtractRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"type\": \"array\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    },\n    \"begin\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-update-extract-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: UpdateExtractRequest
---
