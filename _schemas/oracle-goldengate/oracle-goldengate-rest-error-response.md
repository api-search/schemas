---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP status code
  name: code
  type: integer
- description: Error message
  name: message
  type: string
- description: Error severity level
  name: severity
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-error-response-schema.json
slug: oracle-goldengate-rest-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Error severity level\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-error-response-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ErrorResponse
---
