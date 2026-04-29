---
description: A secret stored in BeyondTrust Secrets Safe.
layout: schema
name: Secret
properties_list:
- description: Unique identifier of the secret.
  name: id
  type: string
- description: Title or name of the secret.
  name: title
  type: string
- description: Description of the secret.
  name: description
  type: string
- description: Type of secret.
  name: type
  type: string
- description: Folder organizing this secret.
  name: folderName
  type: string
- description: When the secret was created.
  name: created
  type: string
- description: When the secret was last modified.
  name: lastModified
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-secret-schema.json
slug: beyondtrust-secret
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-secret-schema.json\",\n  \"title\": \"Secret\",\n  \"description\": \"A secret stored in BeyondTrust Secrets Safe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the secret.\",\n      \"example\": \"secret-a1b2c3\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title or name of the secret.\",\n      \"example\": \"database-credentials\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Description of the secret.\",\n      \"example\": \"Production database credentials\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of secret.\",\n      \"enum\": [\n        \"Password\"\
  ,\n        \"Text\",\n        \"File\"\n      ],\n      \"example\": \"Password\"\n    },\n    \"folderName\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Folder organizing this secret.\",\n      \"example\": \"Production\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the secret was created.\",\n      \"example\": \"2025-01-15T00:00:00Z\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the secret was last modified.\",\n      \"example\": \"2026-04-01T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-secret-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: Secret
---
