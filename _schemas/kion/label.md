---
description: A label provides key-value metadata for organizing and categorizing resources within Kion.
layout: schema
name: Kion Label
properties_list:
- description: Internal Kion label ID.
  name: id
  type: integer
- description: Label key.
  name: key
  type: string
- description: Label value.
  name: value
  type: string
- description: Display color for the label.
  name: color
  type: string
- description: Timestamp when the label was created.
  name: created_at
  type: string
provider_name: Kion
provider_slug: kion
schema_file: json-schema/label.json
slug: label
source_filename: label.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kion/blob/main/json-schema/label.json\",\n  \"title\": \"Kion Label\",\n  \"description\": \"A label provides key-value metadata for organizing and categorizing resources within Kion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Kion label ID.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Label key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Label value.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Display color for the label.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the label was created.\"\n    }\n  },\n  \"required\": [\"key\", \"value\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/json-schema/label.json
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
title: Kion Label
---
