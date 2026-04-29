---
description: Management policy for a certificate.
layout: schema
name: CertificatePolicy
properties_list:
- description: ''
  name: id
  type: string
- description: Properties of the key pair.
  name: key_props
  type: object
- description: Properties of the secret backing a certificate.
  name: secret_props
  type: object
- description: Properties of the X509 component.
  name: x509_props
  type: object
- description: Parameters for the issuer of the X509 component.
  name: issuer
  type: object
- description: ''
  name: lifetime_actions
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-certificate-policy-schema.json
slug: azure-key-vault-certificate-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificatePolicy\",\n  \"type\": \"object\",\n  \"description\": \"Management policy for a certificate.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"key_props\": {\n      \"type\": \"object\",\n      \"description\": \"Properties of the key pair.\"\n    },\n    \"secret_props\": {\n      \"type\": \"object\",\n      \"description\": \"Properties of the secret backing a certificate.\"\n    },\n    \"x509_props\": {\n      \"type\": \"object\",\n      \"description\": \"Properties of the X509 component.\"\n    },\n    \"issuer\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters for the issuer of the X509 component.\"\n    },\n    \"lifetime_actions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-certificate-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CertificatePolicy
---
