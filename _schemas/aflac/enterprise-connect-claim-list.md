---
description: Paginated list of claims.
layout: schema
name: ClaimList
properties_list:
- description: Array of claim records.
  name: items
  type: array
- description: Total number of matching claims.
  name: total
  type: integer
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-claim-list-schema.json
slug: enterprise-connect-claim-list
source_filename: enterprise-connect-claim-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-list-schema.json\",\n  \"title\": \"ClaimList\",\n  \"description\": \"Paginated list of claims.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of claim records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Claim\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching claims.\",\n      \"example\": 30\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-list-schema.json
tags: []
title: ClaimList
---
