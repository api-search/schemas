---
description: ''
layout: schema
name: BulkPointResult
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: Geo Id
  type: string
- description: ''
  name: Geo JSON
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-asset-registry-bulkpointresult-schema.json
slug: agstack-asset-registry-bulkpointresult
source_filename: agstack-asset-registry-bulkpointresult-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/BulkPointResult.json\",\n  \"title\": \"BulkPointResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"created\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Point registered successfully.\"\n    },\n    \"Geo Id\": {\n      \"type\": \"string\"\n    },\n    \"Geo JSON\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-asset-registry-bulkpointresult-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: BulkPointResult
---
