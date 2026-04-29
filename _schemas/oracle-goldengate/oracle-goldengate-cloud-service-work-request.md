---
description: ''
layout: schema
name: WorkRequest
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: operationType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: percentComplete
  type: number
- description: ''
  name: timeAccepted
  type: string
- description: ''
  name: timeStarted
  type: string
- description: ''
  name: timeFinished
  type: string
- description: ''
  name: resources
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-work-request-schema.json
slug: oracle-goldengate-cloud-service-work-request
source_filename: oracle-goldengate-cloud-service-work-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"operationType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"percentComplete\": {\n      \"type\": \"number\"\n    },\n    \"timeAccepted\": {\n      \"type\": \"string\"\n    },\n    \"timeStarted\": {\n      \"type\": \"string\"\n    },\n    \"timeFinished\": {\n      \"type\": \"string\"\n    },\n    \"resources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-work-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: WorkRequest
---
