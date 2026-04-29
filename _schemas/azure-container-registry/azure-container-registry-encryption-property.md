---
description: EncryptionProperty schema from Azure Container Registry API
layout: schema
name: EncryptionProperty
properties_list:
- description: Key vault properties.
  name: keyVaultProperties
  type: object
- description: Indicates whether or not the encryption is enabled for container registry.
  name: status
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-encryption-property-schema.json
slug: azure-container-registry-encryption-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-encryption-property-schema.json\",\n  \"title\": \"EncryptionProperty\",\n  \"description\": \"EncryptionProperty schema from Azure Container Registry API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyVaultProperties\": {\n      \"$ref\": \"#/definitions/KeyVaultProperties\",\n      \"description\": \"Key vault properties.\"\n    },\n    \"status\": {\n      \"description\": \"Indicates whether or not the encryption is enabled for container registry.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"EncryptionStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-encryption-property-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EncryptionProperty
---
