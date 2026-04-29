---
description: ''
layout: schema
name: UpdateServiceRequest
properties_list:
- description: ''
  name: port
  type: integer
- description: ''
  name: secure
  type: boolean
- description: ''
  name: status
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-update-service-request-schema.json
slug: oracle-goldengate-rest-update-service-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateServiceRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"secure\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-update-service-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: UpdateServiceRequest
---
