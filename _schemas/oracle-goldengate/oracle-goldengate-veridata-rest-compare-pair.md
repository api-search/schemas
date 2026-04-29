---
description: ''
layout: schema
name: ComparePair
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: groupId
  type: integer
- description: ''
  name: sourceSchema
  type: string
- description: ''
  name: sourceTable
  type: string
- description: ''
  name: targetSchema
  type: string
- description: ''
  name: targetTable
  type: string
- description: ''
  name: profileId
  type: integer
- description: ''
  name: columnMappings
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-compare-pair-schema.json
slug: oracle-goldengate-veridata-rest-compare-pair
source_filename: oracle-goldengate-veridata-rest-compare-pair-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComparePair\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"groupId\": {\n      \"type\": \"integer\"\n    },\n    \"sourceSchema\": {\n      \"type\": \"string\"\n    },\n    \"sourceTable\": {\n      \"type\": \"string\"\n    },\n    \"targetSchema\": {\n      \"type\": \"string\"\n    },\n    \"targetTable\": {\n      \"type\": \"string\"\n    },\n    \"profileId\": {\n      \"type\": \"integer\"\n    },\n    \"columnMappings\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-compare-pair-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ComparePair
---
