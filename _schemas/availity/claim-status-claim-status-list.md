---
description: ClaimStatusList schema from Availity API
layout: schema
name: ClaimStatusList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-claim-status-list-schema.json
slug: claim-status-claim-status-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-list-schema.json\",\n  \"title\": \"ClaimStatusList\",\n  \"description\": \"ClaimStatusList schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClaimStatusResponse\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-list-schema.json
tags: []
title: ClaimStatusList
---
