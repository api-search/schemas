---
description: The policy rules under which the key can be exported.
layout: schema
name: KeyReleasePolicy
properties_list:
- description: Content type and version of key release policy.
  name: contentType
  type: string
- description: Blob encoding the policy rules under which the key can be released.
  name: data
  type: string
- description: Defines the mutability state of the policy. Once marked immutable, this flag cannot be reset and the policy cannot be changed under any circumstances.
  name: immutable
  type: boolean
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-release-policy-schema.json
slug: azure-key-vault-data-plane-key-release-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyReleasePolicy\",\n  \"type\": \"object\",\n  \"description\": \"The policy rules under which the key can be exported.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"Content type and version of key release policy.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"Blob encoding the policy rules under which the key can be released.\"\n    },\n    \"immutable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Defines the mutability state of the policy. Once marked immutable, this flag cannot be reset and the policy cannot be changed under any circumstances.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-release-policy-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyReleasePolicy
---
