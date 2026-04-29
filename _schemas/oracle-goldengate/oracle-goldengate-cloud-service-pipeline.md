---
description: ''
layout: schema
name: Pipeline
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: sourceConnectionDetailId
  type: string
- description: ''
  name: targetConnectionDetailId
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: timeUpdated
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-pipeline-schema.json
slug: oracle-goldengate-cloud-service-pipeline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"sourceConnectionDetailId\": {\n      \"type\": \"string\"\n    },\n    \"targetConnectionDetailId\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-pipeline-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Pipeline
---
