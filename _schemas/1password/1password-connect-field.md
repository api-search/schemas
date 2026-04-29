---
description: Represents a field within an item that stores a value such as a username, password, or other data.
layout: schema
name: Field
properties_list:
- description: The unique identifier for the field.
  name: id
  type: string
- description: ''
  name: section
  type: object
- description: The type of the field.
  name: type
  type: string
- description: The purpose of the field, indicating its role within the item.
  name: purpose
  type: string
- description: The human-readable label for the field.
  name: label
  type: string
- description: The value stored in the field.
  name: value
  type: string
- description: Whether the field value should be auto-generated.
  name: generate
  type: boolean
- description: The entropy (strength) of the generated value.
  name: entropy
  type: number
- description: ''
  name: recipe
  type: object
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-field-schema.json
slug: 1password-connect-field
source_filename: 1password-connect-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-field-schema.json\",\n  \"title\": \"Field\",\n  \"description\": \"Represents a field within an item that stores a value such as a username, password, or other data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the field.\"\n    },\n    \"section\": {\n      \"$ref\": \"#/components/schemas/SectionRef\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the field.\",\n      \"enum\": [\n        \"STRING\",\n        \"EMAIL\",\n        \"CONCEALED\",\n        \"URL\",\n        \"TOTP\",\n        \"DATE\",\n        \"MONTH_YEAR\",\n        \"MENU\"\n      ]\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"description\": \"The purpose of\
  \ the field, indicating its role within the item.\",\n      \"enum\": [\n        \"USERNAME\",\n        \"PASSWORD\",\n        \"NOTES\"\n      ]\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label for the field.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value stored in the field.\"\n    },\n    \"generate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the field value should be auto-generated.\"\n    },\n    \"entropy\": {\n      \"type\": \"number\",\n      \"description\": \"The entropy (strength) of the generated value.\"\n    },\n    \"recipe\": {\n      \"$ref\": \"#/components/schemas/GeneratorRecipe\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-field-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Field
---
