---
description: ''
layout: schema
name: DatasetField
properties_list:
- description: The field name.
  name: name
  type: string
- description: The display name of the field.
  name: displayName
  type: string
- description: The ordinal position of the field.
  name: ordinal
  type: integer
- description: The data type of the field.
  name: type
  type: object
- description: ''
  name: required
  type: boolean
- description: ''
  name: externalId
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-dataset-field-schema.json
slug: prismAnalytics-dataset-field
source_filename: prismAnalytics-dataset-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatasetField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The field name.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the field.\"\n    },\n    \"ordinal\": {\n      \"type\": \"integer\",\n      \"description\": \"The ordinal position of the field.\"\n    },\n    \"type\": {\n      \"type\": \"object\",\n      \"description\": \"The data type of the field.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-dataset-field-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DatasetField
---
