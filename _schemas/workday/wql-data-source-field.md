---
description: ''
layout: schema
name: DataSourceField
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The alias used to reference this field in WQL queries.
  name: alias
  type: string
- description: The column name for the field.
  name: columnName
  type: string
- description: The data type of the field (e.g., Text, Numeric, Date, Boolean).
  name: type
  type: string
- description: ''
  name: isRequired
  type: boolean
- description: ''
  name: isSortable
  type: boolean
- description: ''
  name: isFilterable
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/wql-data-source-field-schema.json
slug: wql-data-source-field
source_filename: wql-data-source-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"The alias used to reference this field in WQL queries.\"\n    },\n    \"columnName\": {\n      \"type\": \"string\",\n      \"description\": \"The column name for the field.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the field (e.g., Text, Numeric, Date, Boolean).\"\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"isSortable\": {\n      \"type\": \"boolean\"\n    },\n    \"isFilterable\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/wql-data-source-field-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DataSourceField
---
