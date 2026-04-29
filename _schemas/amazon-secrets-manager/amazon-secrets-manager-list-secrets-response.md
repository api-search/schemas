---
description: ListSecretsResponse schema from Amazon Secrets Manager API
layout: schema
name: ListSecretsResponse
properties_list:
- description: ''
  name: SecretList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-list-secrets-response-schema.json
slug: amazon-secrets-manager-list-secrets-response
source_filename: amazon-secrets-manager-list-secrets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-list-secrets-response-schema.json\",\n  \"title\": \"ListSecretsResponse\",\n  \"description\": \"ListSecretsResponse schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecretList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Secret\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-list-secrets-response-schema.json
tags:
- AWS
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: ListSecretsResponse
---
