---
description: A custom field definition for an Intralinks workspace, allowing additional metadata to be attached to documents, folders, and groups.
layout: schema
name: Intralinks Custom Field
properties_list:
- description: Unique identifier of the custom field.
  name: id
  type: string
- description: Custom field name.
  name: name
  type: string
- description: Custom field data type.
  name: type
  type: string
- description: Whether the field is mandatory.
  name: isRequired
  type: boolean
- description: Available options for SELECT type fields.
  name: options
  type: array
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/custom-field.json
slug: custom-field
source_filename: custom-field.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"custom-field.json\",\n  \"title\": \"Intralinks Custom Field\",\n  \"description\": \"A custom field definition for an Intralinks workspace, allowing additional metadata to be attached to documents, folders, and groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the custom field.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Custom field name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"TEXT\", \"DATE\", \"SELECT\"],\n      \"description\": \"Custom field data type.\"\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the field is mandatory.\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Available\
  \ options for SELECT type fields.\"\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/custom-field.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Custom Field
---
