---
description: Tag schema from Amazon Secrets Manager API
layout: schema
name: Tag
properties_list:
- description: The key identifier or name of the tag.
  name: Key
  type: string
- description: The string value associated with the key of the tag.
  name: Value
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-tag-schema.json
slug: amazon-secrets-manager-tag
source_filename: amazon-secrets-manager-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The key identifier or name of the tag.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The string value associated with the key of the tag.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-tag-schema.json
tags:
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: Tag
---
