---
description: A dimension value used for filtering and reporting.
layout: schema
name: DimensionValue
properties_list:
- description: The name of the dimension.
  name: dimensionName
  type: string
- description: The value of the dimension.
  name: value
  type: string
- description: The ID associated with the value.
  name: id
  type: string
- description: Match type for filtering.
  name: matchType
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-dimension-value-schema.json
slug: google-campaign-manager-dimension-value
source_filename: google-campaign-manager-dimension-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DimensionValue\",\n  \"type\": \"object\",\n  \"description\": \"A dimension value used for filtering and reporting.\",\n  \"properties\": {\n    \"dimensionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dimension.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the dimension.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID associated with the value.\"\n    },\n    \"matchType\": {\n      \"type\": \"string\",\n      \"description\": \"Match type for filtering.\"\n    },\n    \"etag\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-dimension-value-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: DimensionValue
---
