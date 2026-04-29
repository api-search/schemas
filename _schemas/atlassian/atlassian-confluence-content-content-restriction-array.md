---
description: ''
layout: schema
name: ContentRestrictionArray
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
- description: This property is used by the UI to figure out whether a set of restrictions has changed.
  name: restrictionsHash
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-restriction-array-schema.json
slug: atlassian-confluence-content-content-restriction-array
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentRestrictionArray\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\"\n    },\n    \"start\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    },\n    \"restrictionsHash\": {\n      \"type\": \"string\",\n      \"description\": \"This property is used by the UI to figure out whether a set of restrictions\\nhas changed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-restriction-array-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentRestrictionArray
---
