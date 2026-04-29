---
description: ''
layout: schema
name: Job
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: groupIds
  type: array
- description: ''
  name: profileId
  type: integer
- description: ''
  name: status
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-job-schema.json
slug: oracle-goldengate-veridata-rest-job
source_filename: oracle-goldengate-veridata-rest-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"groupIds\": {\n      \"type\": \"array\"\n    },\n    \"profileId\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-job-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Job
---
