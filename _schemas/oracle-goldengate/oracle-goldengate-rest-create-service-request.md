---
description: ''
layout: schema
name: CreateServiceRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: secure
  type: boolean
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-service-request-schema.json
slug: oracle-goldengate-rest-create-service-request
source_filename: oracle-goldengate-rest-create-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateServiceRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"secure\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-service-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateServiceRequest
---
