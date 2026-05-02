---
description: A certificate bundle consists of a certificate (X509) plus its attributes.
layout: schema
name: CertificateBundle
properties_list:
- description: The certificate id.
  name: id
  type: string
- description: The key id.
  name: kid
  type: string
- description: The secret id.
  name: sid
  type: string
- description: Thumbprint of the certificate.
  name: x5t
  type: string
- description: CER contents of x509 certificate.
  name: cer
  type: string
- description: The content type of the secret.
  name: contentType
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-bundle-schema.json
slug: azure-key-vault-data-plane-certificate-bundle
source_filename: azure-key-vault-data-plane-certificate-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateBundle\",\n  \"type\": \"object\",\n  \"description\": \"A certificate bundle consists of a certificate (X509) plus its attributes.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate id.\"\n    },\n    \"kid\": {\n      \"type\": \"string\",\n      \"description\": \"The key id.\"\n    },\n    \"sid\": {\n      \"type\": \"string\",\n      \"description\": \"The secret id.\"\n    },\n    \"x5t\": {\n      \"type\": \"string\",\n      \"description\": \"Thumbprint of the certificate.\"\n    },\n    \"cer\": {\n      \"type\": \"string\",\n      \"description\": \"CER contents of x509 certificate.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the secret.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata\
  \ in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-bundle-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificateBundle
---
