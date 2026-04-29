---
description: ''
layout: schema
name: UserArray
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: start
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: size
  type: integer
- description: This property will return total count of the objects before pagination is applied. This value is returned if `shouldReturnTotalSize` is set to `true`.
  name: totalSize
  type: integer
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-user-array-schema.json
slug: atlassian-confluence-content-user-array
source_filename: atlassian-confluence-content-user-array-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserArray\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\"\n    },\n    \"start\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"description\": \"This property will return total count of the objects before pagination is applied.\\nThis value is returned if `shouldReturnTotalSize` is set to `true`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-user-array-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: UserArray
---
