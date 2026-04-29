---
description: ''
layout: schema
name: CreateConnectionRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: connectionString
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-connection-request-schema.json
slug: oracle-goldengate-rest-create-connection-request
source_filename: oracle-goldengate-rest-create-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateConnectionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"connectionString\": {\n      \"type\": \"string\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-connection-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateConnectionRequest
---
