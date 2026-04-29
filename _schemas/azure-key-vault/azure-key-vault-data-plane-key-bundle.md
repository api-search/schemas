---
description: A KeyBundle consisting of a WebKey plus its attributes.
layout: schema
name: KeyBundle
properties_list:
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: True if the key's lifetime is managed by key vault. If this is a key backing a certificate, then managed will be true.
  name: managed
  type: boolean
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-key-bundle-schema.json
slug: azure-key-vault-data-plane-key-bundle
source_filename: azure-key-vault-data-plane-key-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyBundle\",\n  \"type\": \"object\",\n  \"description\": \"A KeyBundle consisting of a WebKey plus its attributes.\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the key's lifetime is managed by key vault. If this is a key backing a certificate, then managed will be true.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-key-bundle-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: KeyBundle
---
