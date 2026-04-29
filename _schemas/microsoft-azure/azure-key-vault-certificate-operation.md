---
description: A certificate operation is returned in case of asynchronous requests.
layout: schema
name: CertificateOperation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: issuer
  type: object
- description: The certificate signing request (CSR) in base64.
  name: csr
  type: string
- description: ''
  name: cancellation_requested
  type: boolean
- description: ''
  name: status
  type: string
- description: ''
  name: status_details
  type: string
- description: ''
  name: error
  type: object
- description: ''
  name: target
  type: string
- description: ''
  name: request_id
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-certificate-operation-schema.json
slug: azure-key-vault-certificate-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateOperation\",\n  \"type\": \"object\",\n  \"description\": \"A certificate operation is returned in case of asynchronous requests.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"type\": \"object\"\n    },\n    \"csr\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate signing request (CSR) in base64.\"\n    },\n    \"cancellation_requested\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"status_details\": {\n      \"type\": \"string\"\n    },\n    \"error\": {\n      \"type\": \"object\"\n    },\n    \"target\": {\n      \"type\": \"string\"\n    },\n    \"request_id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-certificate-operation-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CertificateOperation
---
