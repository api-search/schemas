---
description: The certificate import parameters.
layout: schema
name: CertificateImportParameters
properties_list:
- description: Base64 encoded representation of the certificate object to import. This certificate needs to contain the private key.
  name: value
  type: string
- description: If the private key in base64EncodedCertificate is encrypted, the password used for encryption.
  name: pwd
  type: string
- description: Application specific metadata in the form of key-value pairs.
  name: tags
  type: object
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-certificate-import-parameters-schema.json
slug: azure-key-vault-data-plane-certificate-import-parameters
source_filename: azure-key-vault-data-plane-certificate-import-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateImportParameters\",\n  \"type\": \"object\",\n  \"description\": \"The certificate import parameters.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Base64 encoded representation of the certificate object to import. This certificate needs to contain the private key.\"\n    },\n    \"pwd\": {\n      \"type\": \"string\",\n      \"description\": \"If the private key in base64EncodedCertificate is encrypted, the password used for encryption.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Application specific metadata in the form of key-value pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-certificate-import-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: CertificateImportParameters
---
