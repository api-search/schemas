---
description: ''
layout: schema
name: Table
properties_list:
- description: The Workday ID of the table.
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The name of the table.
  name: name
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: fields
  type: array
- description: ''
  name: isAccessible
  type: boolean
- description: ''
  name: documentCount
  type: integer
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-table-schema.json
slug: prismAnalytics-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the table.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"fields\": {\n      \"type\": \"array\"\n    },\n    \"isAccessible\": {\n      \"type\": \"boolean\"\n    },\n    \"documentCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-table-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Table
---
