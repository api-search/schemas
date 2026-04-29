---
description: A secret including its sensitive value.
layout: schema
name: SecretWithValue
properties_list:
- description: Unique identifier.
  name: id
  type: string
- description: Secret title.
  name: title
  type: string
- description: Secret type.
  name: type
  type: string
- description: Password value (for Password type secrets).
  name: password
  type: string
- description: Text value (for Text type secrets).
  name: text
  type: string
- description: Folder name.
  name: folderName
  type: string
- description: Creation timestamp.
  name: created
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-secret-with-value-schema.json
slug: beyondtrust-secret-with-value
source_filename: beyondtrust-secret-with-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-secret-with-value-schema.json\",\n  \"title\": \"SecretWithValue\",\n  \"description\": \"A secret including its sensitive value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier.\",\n      \"example\": \"secret-a1b2c3\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Secret title.\",\n      \"example\": \"database-credentials\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Secret type.\",\n      \"example\": \"Password\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Password value (for Password type secrets).\",\n      \"example\": \"Xk2!mP9@nQ7#rT5\"\n    },\n    \"text\": {\n\
  \      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Text value (for Text type secrets).\",\n      \"example\": null\n    },\n    \"folderName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Folder name.\",\n      \"example\": \"Production\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\",\n      \"example\": \"2025-01-15T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-secret-with-value-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: SecretWithValue
---
