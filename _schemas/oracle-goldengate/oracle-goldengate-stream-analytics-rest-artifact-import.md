---
description: JSON document containing exported GGSA artifacts
layout: schema
name: ArtifactImport
properties_list:
- description: ''
  name: pipeline
  type: object
- description: ''
  name: connections
  type: array
- description: ''
  name: references
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-stream-analytics-rest-artifact-import-schema.json
slug: oracle-goldengate-stream-analytics-rest-artifact-import
source_filename: oracle-goldengate-stream-analytics-rest-artifact-import-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ArtifactImport\",\n  \"type\": \"object\",\n  \"description\": \"JSON document containing exported GGSA artifacts\",\n  \"properties\": {\n    \"pipeline\": {\n      \"type\": \"object\"\n    },\n    \"connections\": {\n      \"type\": \"array\"\n    },\n    \"references\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-stream-analytics-rest-artifact-import-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ArtifactImport
---
