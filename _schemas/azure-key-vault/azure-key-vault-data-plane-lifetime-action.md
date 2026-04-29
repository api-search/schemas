---
description: Action and its trigger that will be performed by Key Vault over the lifetime of a certificate.
layout: schema
name: LifetimeAction
properties_list:
- description: The condition that will execute the action.
  name: trigger
  type: object
- description: The action that will be executed.
  name: action
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-lifetime-action-schema.json
slug: azure-key-vault-data-plane-lifetime-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifetimeAction\",\n  \"type\": \"object\",\n  \"description\": \"Action and its trigger that will be performed by Key Vault over the lifetime of a certificate.\",\n  \"properties\": {\n    \"trigger\": {\n      \"type\": \"object\",\n      \"description\": \"The condition that will execute the action.\"\n    },\n    \"action\": {\n      \"type\": \"object\",\n      \"description\": \"The action that will be executed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-lifetime-action-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: LifetimeAction
---
