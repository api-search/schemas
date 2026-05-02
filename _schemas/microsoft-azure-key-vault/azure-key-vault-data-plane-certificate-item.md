---
description: The certificate item containing certificate metadata.
layout: schema
name: CertificateItem
properties_list:
- description: Certificate identifier.
  name: id
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
- description: Thumbprint of the certificate.
  name: x5t
  type: string
- description: The subject name of the certificate.
  name: subject
  type: string
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-item-schema.json
slug: azure-key-vault-data-plane-certificate-item
source_filename: azure-key-vault-data-plane-certificate-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateItem\",\n  \"type\": \"object\",\n  \"description\": \"The certificate item containing certificate metadata.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate identifier.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    },\n    \"x5t\": {\n      \"type\": \"string\",\n      \"description\": \"Thumbprint of the certificate.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject name of the certificate.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-item-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificateItem
---
