---
description: ''
layout: schema
name: ColumnMapping
properties_list:
- description: ''
  name: sourceColumn
  type: string
- description: ''
  name: targetColumn
  type: string
- description: ''
  name: dataType
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-column-mapping-schema.json
slug: oracle-goldengate-veridata-rest-column-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnMapping\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceColumn\": {\n      \"type\": \"string\"\n    },\n    \"targetColumn\": {\n      \"type\": \"string\"\n    },\n    \"dataType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-column-mapping-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ColumnMapping
---
