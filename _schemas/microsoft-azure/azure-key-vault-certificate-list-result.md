---
description: The certificate list result.
layout: schema
name: CertificateListResult
properties_list:
- description: A list of certificates.
  name: value
  type: array
- description: The URL to get the next set of certificates.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-certificate-list-result-schema.json
slug: azure-key-vault-certificate-list-result
source_filename: azure-key-vault-certificate-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateListResult\",\n  \"type\": \"object\",\n  \"description\": \"The certificate list result.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"A list of certificates.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to get the next set of certificates.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-certificate-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CertificateListResult
---
