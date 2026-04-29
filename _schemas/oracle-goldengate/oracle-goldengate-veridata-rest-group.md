---
description: ''
layout: schema
name: Group
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
  name: sourceConnectionId
  type: integer
- description: ''
  name: targetConnectionId
  type: integer
- description: ''
  name: profileId
  type: integer
- description: ''
  name: comparePairCount
  type: integer
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-group-schema.json
slug: oracle-goldengate-veridata-rest-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"sourceConnectionId\": {\n      \"type\": \"integer\"\n    },\n    \"targetConnectionId\": {\n      \"type\": \"integer\"\n    },\n    \"profileId\": {\n      \"type\": \"integer\"\n    },\n    \"comparePairCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-group-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Group
---
