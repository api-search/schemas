---
description: Paginated list of policies.
layout: schema
name: PolicyList
properties_list:
- description: Array of policy records.
  name: items
  type: array
- description: Total number of matching policies.
  name: total
  type: integer
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-policy-list-schema.json
slug: enterprise-connect-policy-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-policy-list-schema.json\",\n  \"title\": \"PolicyList\",\n  \"description\": \"Paginated list of policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of policy records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Policy\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching policies.\",\n      \"example\": 75\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-policy-list-schema.json
tags: []
title: PolicyList
---
