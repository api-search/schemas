---
description: ''
layout: schema
name: Profile
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
  name: comparisonMethod
  type: string
- description: ''
  name: maxConcurrentComparePairs
  type: integer
- description: ''
  name: deltaProcessing
  type: boolean
- description: ''
  name: reportOutOfSync
  type: boolean
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-profile-schema.json
slug: oracle-goldengate-veridata-rest-profile
source_filename: oracle-goldengate-veridata-rest-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"comparisonMethod\": {\n      \"type\": \"string\"\n    },\n    \"maxConcurrentComparePairs\": {\n      \"type\": \"integer\"\n    },\n    \"deltaProcessing\": {\n      \"type\": \"boolean\"\n    },\n    \"reportOutOfSync\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-profile-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Profile
---
