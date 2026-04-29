---
description: ''
layout: schema
name: ReplaceComparePairRequest
properties_list:
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
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-replace-compare-pair-request-schema.json
slug: oracle-goldengate-veridata-rest-replace-compare-pair-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceComparePairRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceSchema\": {\n      \"type\": \"string\"\n    },\n    \"sourceTable\": {\n      \"type\": \"string\"\n    },\n    \"targetSchema\": {\n      \"type\": \"string\"\n    },\n    \"targetTable\": {\n      \"type\": \"string\"\n    },\n    \"profileId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-replace-compare-pair-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ReplaceComparePairRequest
---
