---
description: The list of credential result response.
layout: schema
name: CredentialResults
properties_list:
- description: The list of kubeconfigs.
  name: kubeconfigs
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-credential-results-schema.json
slug: azure-kubernetes-service-credential-results
source_filename: azure-kubernetes-service-credential-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CredentialResults\",\n  \"type\": \"object\",\n  \"description\": \"The list of credential result response.\",\n  \"properties\": {\n    \"kubeconfigs\": {\n      \"type\": \"array\",\n      \"description\": \"The list of kubeconfigs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-credential-results-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CredentialResults
---
