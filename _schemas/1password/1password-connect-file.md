---
description: Represents a file attached to an item in a vault.
layout: schema
name: File
properties_list:
- description: The unique identifier for the file.
  name: id
  type: string
- description: The name of the file.
  name: name
  type: string
- description: The size of the file in bytes.
  name: size
  type: integer
- description: The API path to retrieve the file content.
  name: content_path
  type: string
- description: ''
  name: section
  type: object
- description: The base64-encoded file content, included when inline_files is true.
  name: content
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-file-schema.json
slug: 1password-connect-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-file-schema.json\",\n  \"title\": \"File\",\n  \"description\": \"Represents a file attached to an item in a vault.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the file.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the file in bytes.\"\n    },\n    \"content_path\": {\n      \"type\": \"string\",\n      \"description\": \"The API path to retrieve the file content.\"\n    },\n    \"section\": {\n      \"$ref\": \"#/components/schemas/SectionRef\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"\
  format\": \"byte\",\n      \"description\": \"The base64-encoded file content, included when inline_files is true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-file-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: File
---
