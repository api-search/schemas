---
description: An object that represents a container registry.
layout: schema
name: Registry
properties_list:
- description: The identity of the container registry.
  name: identity
  type: object
- description: The properties of the container registry.
  name: properties
  type: object
- description: The SKU of the container registry.
  name: sku
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-registry-schema.json
slug: azure-container-registry-registry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-schema.json\",\n  \"title\": \"Registry\",\n  \"description\": \"An object that represents a container registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identity\": {\n      \"$ref\": \"#/definitions/IdentityProperties\",\n      \"description\": \"The identity of the container registry.\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/RegistryProperties\",\n      \"description\": \"The properties of the container registry.\",\n      \"x-ms-client-flatten\": true\n    },\n    \"sku\": {\n      \"$ref\": \"#/definitions/Sku\",\n      \"description\": \"The SKU of the container registry.\"\n    }\n  },\n  \"required\": [\n    \"sku\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-registry-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Registry
---
