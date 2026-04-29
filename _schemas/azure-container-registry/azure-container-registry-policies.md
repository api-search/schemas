---
description: The policies for a container registry.
layout: schema
name: Policies
properties_list:
- description: The quarantine policy for a container registry.
  name: quarantinePolicy
  type: object
- description: The retention policy for a container registry.
  name: retentionPolicy
  type: object
- description: The content trust policy for a container registry.
  name: trustPolicy
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-policies-schema.json
slug: azure-container-registry-policies
source_filename: azure-container-registry-policies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-policies-schema.json\",\n  \"title\": \"Policies\",\n  \"description\": \"The policies for a container registry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quarantinePolicy\": {\n      \"$ref\": \"#/definitions/QuarantinePolicy\",\n      \"description\": \"The quarantine policy for a container registry.\"\n    },\n    \"retentionPolicy\": {\n      \"$ref\": \"#/definitions/RetentionPolicy\",\n      \"description\": \"The retention policy for a container registry.\"\n    },\n    \"trustPolicy\": {\n      \"$ref\": \"#/definitions/TrustPolicy\",\n      \"description\": \"The content trust policy for a container registry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-policies-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Policies
---
