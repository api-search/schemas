---
description: Management policy for a certificate.
layout: schema
name: CertificatePolicy
properties_list:
- description: The certificate id.
  name: id
  type: string
- description: Actions that will be performed by Key Vault over the lifetime of a certificate.
  name: lifetime_actions
  type: array
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-policy-schema.json
slug: azure-key-vault-data-plane-certificate-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificatePolicy\",\n  \"type\": \"object\",\n  \"description\": \"Management policy for a certificate.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate id.\"\n    },\n    \"lifetime_actions\": {\n      \"type\": \"array\",\n      \"description\": \"Actions that will be performed by Key Vault over the lifetime of a certificate.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-policy-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificatePolicy
---
