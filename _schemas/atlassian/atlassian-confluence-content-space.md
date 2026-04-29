---
description: ''
layout: schema
name: Space
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: operations
  type: array
- description: ''
  name: permissions
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: history
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-space-schema.json
slug: atlassian-confluence-content-space
source_filename: atlassian-confluence-content-space-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"object\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"permissions\": {\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"history\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-space-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Space
---
