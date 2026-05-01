---
description: Response for listing configured tables.
layout: schema
name: ListConfiguredTablesResponse
properties_list:
- description: The token value retrieved from a previous paginated request.
  name: nextToken
  type: string
- description: The list of configured tables.
  name: configuredTableList
  type: array
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-list-configured-tables-response-schema.json
slug: clean-rooms-list-configured-tables-response
source_filename: clean-rooms-list-configured-tables-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-configured-tables-response-schema.json\",\n  \"title\": \"ListConfiguredTablesResponse\",\n  \"description\": \"Response for listing configured tables.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token value retrieved from a previous paginated request.\"\n    },\n    \"configuredTableList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfiguredTable\"\n      },\n      \"description\": \"The list of configured tables.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-list-configured-tables-response-schema.json
tags:
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: ListConfiguredTablesResponse
---
