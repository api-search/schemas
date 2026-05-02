---
description: The certificate update parameters.
layout: schema
name: CertificateUpdateParameters
properties_list:
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-update-parameters-schema.json
slug: azure-key-vault-data-plane-certificate-update-parameters
source_filename: azure-key-vault-data-plane-certificate-update-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateUpdateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The certificate update parameters.\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-update-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificateUpdateParameters
---
