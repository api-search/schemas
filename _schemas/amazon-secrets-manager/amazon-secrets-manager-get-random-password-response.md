---
description: GetRandomPasswordResponse schema from Amazon Secrets Manager API
layout: schema
name: GetRandomPasswordResponse
properties_list:
- description: A string with the password.
  name: RandomPassword
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-get-random-password-response-schema.json
slug: amazon-secrets-manager-get-random-password-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-get-random-password-response-schema.json\",\n  \"title\": \"GetRandomPasswordResponse\",\n  \"description\": \"GetRandomPasswordResponse schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RandomPassword\": {\n      \"type\": \"string\",\n      \"description\": \"A string with the password.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-get-random-password-response-schema.json
tags:
- AWS
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: GetRandomPasswordResponse
---
