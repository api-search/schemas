---
description: A Zesty.io field defines a single data attribute within a content model, specifying its type, validation rules, and display settings.
layout: schema
name: Zesty Field
properties_list:
- description: The Zesty Universal Identifier for the field.
  name: ZUID
  type: string
- description: The content model ZUID this field belongs to.
  name: contentModelZUID
  type: string
- description: The programmatic name of the field.
  name: name
  type: string
- description: The display label for the field.
  name: label
  type: string
- description: A description of the field.
  name: description
  type: string
- description: The data type of the field (e.g., text, textarea, wysiwyg_basic, images, date, number, link, internal_link, one_to_one, one_to_many).
  name: datatype
  type: string
- description: Whether the field is required.
  name: required
  type: boolean
- description: The sort order of the field within the model.
  name: sort
  type: integer
- description: Additional field settings and validation rules.
  name: settings
  type: object
- description: Timestamp when the field was created.
  name: createdAt
  type: string
- description: Timestamp when the field was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/field.json
slug: field
source_filename: field.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/field.json\",\n  \"title\": \"Zesty Field\",\n  \"description\": \"A Zesty.io field defines a single data attribute within a content model, specifying its type, validation rules, and display settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the field.\"\n    },\n    \"contentModelZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The content model ZUID this field belongs to.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The programmatic name of the field.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display label for the field.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description\
  \ of the field.\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the field (e.g., text, textarea, wysiwyg_basic, images, date, number, link, internal_link, one_to_one, one_to_many).\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the field is required.\"\n    },\n    \"sort\": {\n      \"type\": \"integer\",\n      \"description\": \"The sort order of the field within the model.\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Additional field settings and validation rules.\",\n      \"additionalProperties\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the field was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the field was last updated.\"\n    }\n  },\n  \"\
  required\": [\"ZUID\", \"contentModelZUID\", \"name\", \"datatype\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/field.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Field
---
