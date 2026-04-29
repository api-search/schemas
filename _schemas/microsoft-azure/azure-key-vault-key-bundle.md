---
description: A key bundle containing the key and its attributes.
layout: schema
name: KeyBundle
properties_list:
- description: Application-specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: Whether the key's lifetime is managed by Key Vault.
  name: managed
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-key-bundle-schema.json
slug: azure-key-vault-key-bundle
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyBundle\",\n  \"type\": \"object\",\n  \"description\": \"A key bundle containing the key and its attributes.\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application-specific metadata in the form of key-value pairs.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the key's lifetime is managed by Key Vault.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-key-bundle-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: KeyBundle
---
