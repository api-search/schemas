---
description: The key update parameters.
layout: schema
name: KeyUpdateParameters
properties_list:
- description: JSON web key operations.
  name: key_ops
  type: array
- description: Application-specific metadata.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-update-parameters-schema.json
slug: azure-key-vault-key-update-parameters
source_filename: azure-key-vault-key-update-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyUpdateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The key update parameters.\",\n  \"properties\": {\n    \"key_ops\": {\n      \"type\": \"array\",\n      \"description\": \"JSON web key operations.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-update-parameters-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyUpdateParameters
---
