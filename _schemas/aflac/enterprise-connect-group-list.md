---
description: Paginated list of employer groups.
layout: schema
name: GroupList
properties_list:
- description: Array of group records.
  name: items
  type: array
- description: Total number of groups.
  name: total
  type: integer
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-group-list-schema.json
slug: enterprise-connect-group-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-group-list-schema.json\",\n  \"title\": \"GroupList\",\n  \"description\": \"Paginated list of employer groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Array of group records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Group\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of groups.\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-group-list-schema.json
tags: []
title: GroupList
---
