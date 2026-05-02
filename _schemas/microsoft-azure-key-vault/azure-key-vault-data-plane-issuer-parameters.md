---
description: Parameters for the issuer of the X509 component of a certificate.
layout: schema
name: IssuerParameters
properties_list:
- description: Name of the referenced issuer object or reserved names; for example, 'Self' or 'Unknown'.
  name: name
  type: string
- description: Certificate type as supported by the provider (optional); for example 'OV-SSL', 'EV-SSL'.
  name: cty
  type: string
- description: Indicates if the certificates generated under this policy should be published to certificate transparency logs.
  name: cert_transparency
  type: boolean
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-issuer-parameters-schema.json
slug: azure-key-vault-data-plane-issuer-parameters
source_filename: azure-key-vault-data-plane-issuer-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssuerParameters\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for the issuer of the X509 component of a certificate.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the referenced issuer object or reserved names; for example, 'Self' or 'Unknown'.\"\n    },\n    \"cty\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate type as supported by the provider (optional); for example 'OV-SSL', 'EV-SSL'.\"\n    },\n    \"cert_transparency\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the certificates generated under this policy should be published to certificate transparency logs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-issuer-parameters-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: IssuerParameters
---
