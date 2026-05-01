---
description: UpdateGraphInput schema from Neptune
layout: schema
name: UpdateGraphInput
properties_list:
- description: The new provisioned memory size in NCUs.
  name: provisionedMemory
  type: integer
- description: Whether deletion protection is enabled.
  name: deletionProtection
  type: boolean
- description: ''
  name: publicConnectivity
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-update-graph-input-schema.json
slug: analytics-update-graph-input
source_filename: analytics-update-graph-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-update-graph-input-schema.json\",\n  \"title\": \"UpdateGraphInput\",\n  \"description\": \"UpdateGraphInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"provisionedMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"The new provisioned memory size in NCUs.\"\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion protection is enabled.\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-update-graph-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: UpdateGraphInput
---
