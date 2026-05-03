---
description: Metadata describing a predefined or custom field for apps, users, or contracts in Torii.
layout: schema
name: Torii Field Metadata
properties_list:
- description: Field key identifier.
  name: key
  type: string
- description: Display name of the field.
  name: name
  type: string
- description: Data type of the field.
  name: type
  type: string
- description: Whether this is a custom field.
  name: isCustom
  type: boolean
- description: Whether this field is required.
  name: isRequired
  type: boolean
provider_name: Torii
provider_slug: torii
schema_file: json-schema/field-metadata.json
slug: field-metadata
source_filename: field-metadata.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/field-metadata.json\",\n  \"title\": \"Torii Field Metadata\",\n  \"description\": \"Metadata describing a predefined or custom field for apps, users, or contracts in Torii.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Field key identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the field.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the field.\"\n    },\n    \"isCustom\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a custom field.\"\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this field is required.\"\n    }\n  },\n  \"required\": [\"key\", \"name\",\
  \ \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/field-metadata.json
tags:
- SaaS Management
title: Torii Field Metadata
---
