---
description: Request body for creating a new secret.
layout: schema
name: CreateSecretRequest
properties_list:
- description: Title of the secret.
  name: title
  type: string
- description: Description of the secret.
  name: description
  type: string
- description: Type of secret.
  name: type
  type: string
- description: Password value (for Password type).
  name: password
  type: string
- description: Text value (for Text type).
  name: text
  type: string
- description: Folder to store the secret in.
  name: folderName
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-create-secret-request-schema.json
slug: beyondtrust-create-secret-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-create-secret-request-schema.json\",\n  \"title\": \"CreateSecretRequest\",\n  \"description\": \"Request body for creating a new secret.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the secret.\",\n      \"example\": \"new-api-key\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the secret.\",\n      \"example\": \"API key for production service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of secret.\",\n      \"enum\": [\n        \"Password\",\n        \"Text\",\n        \"File\"\n      ],\n      \"example\": \"Password\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password\
  \ value (for Password type).\",\n      \"example\": \"SecurePassword123!\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Text value (for Text type).\",\n      \"example\": \"my-secret-text\"\n    },\n    \"folderName\": {\n      \"type\": \"string\",\n      \"description\": \"Folder to store the secret in.\",\n      \"example\": \"Production\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-create-secret-request-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CreateSecretRequest
---
