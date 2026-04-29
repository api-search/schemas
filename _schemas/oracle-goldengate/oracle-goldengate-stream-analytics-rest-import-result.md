---
description: ''
layout: schema
name: ImportResult
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: importedArtifacts
  type: integer
- description: ''
  name: messages
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-import-result-schema.json
slug: oracle-goldengate-stream-analytics-rest-import-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\"\n    },\n    \"importedArtifacts\": {\n      \"type\": \"integer\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-import-result-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ImportResult
---
