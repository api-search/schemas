---
description: The secret set parameters.
layout: schema
name: SecretSetParameters
properties_list:
- description: The value of the secret.
  name: value
  type: string
- description: Application-specific metadata.
  name: tags
  type: object
- description: Type of the secret value such as a password.
  name: contentType
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-secret-set-parameters-schema.json
slug: azure-key-vault-secret-set-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecretSetParameters\",\n  \"type\": \"object\",\n  \"description\": \"The secret set parameters.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the secret.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the secret value such as a password.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-secret-set-parameters-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: SecretSetParameters
---
