---
description: The certificate management attributes.
layout: schema
name: CertificateAttributes
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: nbf
  type: integer
- description: ''
  name: exp
  type: integer
- description: ''
  name: created
  type: integer
- description: ''
  name: updated
  type: integer
- description: ''
  name: recoveryLevel
  type: string
- description: ''
  name: recoverableDays
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-certificate-attributes-schema.json
slug: azure-key-vault-certificate-attributes
source_filename: azure-key-vault-certificate-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateAttributes\",\n  \"type\": \"object\",\n  \"description\": \"The certificate management attributes.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"nbf\": {\n      \"type\": \"integer\"\n    },\n    \"exp\": {\n      \"type\": \"integer\"\n    },\n    \"created\": {\n      \"type\": \"integer\"\n    },\n    \"updated\": {\n      \"type\": \"integer\"\n    },\n    \"recoveryLevel\": {\n      \"type\": \"string\"\n    },\n    \"recoverableDays\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-certificate-attributes-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CertificateAttributes
---
