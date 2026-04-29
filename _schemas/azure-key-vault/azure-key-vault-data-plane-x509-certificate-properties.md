---
description: Properties of the X509 component of a certificate.
layout: schema
name: X509CertificateProperties
properties_list:
- description: The subject name. Should be a valid X509 distinguished name.
  name: subject
  type: string
- description: The enhanced key usage.
  name: ekus
  type: array
- description: Defines how the certificate's key may be used.
  name: key_usage
  type: array
- description: The duration that the certificate is valid in months.
  name: validity_months
  type: integer
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-x509-certificate-properties-schema.json
slug: azure-key-vault-data-plane-x509-certificate-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"X509CertificateProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of the X509 component of a certificate.\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject name. Should be a valid X509 distinguished name.\"\n    },\n    \"ekus\": {\n      \"type\": \"array\",\n      \"description\": \"The enhanced key usage.\"\n    },\n    \"key_usage\": {\n      \"type\": \"array\",\n      \"description\": \"Defines how the certificate's key may be used.\"\n    },\n    \"validity_months\": {\n      \"type\": \"integer\",\n      \"description\": \"The duration that the certificate is valid in months.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-x509-certificate-properties-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: X509CertificateProperties
---
