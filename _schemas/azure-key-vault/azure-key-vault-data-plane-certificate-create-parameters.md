---
description: The certificate create parameters.
layout: schema
name: CertificateCreateParameters
properties_list:
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-create-parameters-schema.json
slug: azure-key-vault-data-plane-certificate-create-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateCreateParameters\",\n  \"type\": \"object\",\n  \"description\": \"The certificate create parameters.\",\n  \"properties\": {\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-create-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificateCreateParameters
---
