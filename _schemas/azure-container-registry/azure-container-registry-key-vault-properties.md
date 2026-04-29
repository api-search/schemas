---
description: KeyVaultProperties schema from Azure Container Registry API
layout: schema
name: KeyVaultProperties
properties_list:
- description: The client id of the identity which will be used to access key vault.
  name: identity
  type: string
- description: Key vault uri to access the encryption key.
  name: keyIdentifier
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-key-vault-properties-schema.json
slug: azure-container-registry-key-vault-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-key-vault-properties-schema.json\",\n  \"title\": \"KeyVaultProperties\",\n  \"description\": \"KeyVaultProperties schema from Azure Container Registry API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identity\": {\n      \"description\": \"The client id of the identity which will be used to access key vault.\",\n      \"type\": \"string\"\n    },\n    \"keyIdentifier\": {\n      \"description\": \"Key vault uri to access the encryption key.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-key-vault-properties-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: KeyVaultProperties
---
