---
description: ''
layout: schema
name: LoginResponse
properties_list:
- description: ''
  name: token
  type: string
- description: ''
  name: sessionTimeout
  type: integer
- description: ''
  name: username
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-login-response-schema.json
slug: oracle-goldengate-veridata-rest-login-response
source_filename: oracle-goldengate-veridata-rest-login-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\"\n    },\n    \"sessionTimeout\": {\n      \"type\": \"integer\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-login-response-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: LoginResponse
---
