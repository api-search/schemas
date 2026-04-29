---
description: DestinationPatchRequest schema from Airbyte API
layout: schema
name: DestinationPatchRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: configuration
  type: object
- description: ''
  name: resourceAllocation
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-destination-patch-request-schema.json
slug: airbyte-destination-patch-request
source_filename: airbyte-destination-patch-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-patch-request-schema.json\",\n  \"title\": \"DestinationPatchRequest\",\n  \"description\": \"DestinationPatchRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/DestinationConfiguration\"\n    },\n    \"resourceAllocation\": {\n      \"$ref\": \"#/components/schemas/ScopedResourceRequirements\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-patch-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DestinationPatchRequest
---
