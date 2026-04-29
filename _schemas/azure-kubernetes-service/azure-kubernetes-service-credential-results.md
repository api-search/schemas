---
description: The list of credential result response.
layout: schema
name: CredentialResults
properties_list:
- description: Base64-encoded Kubernetes configuration file.
  name: kubeconfigs
  type: array
provider_name: Azure Kubernetes Service
provider_slug: azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-credential-results-schema.json
slug: azure-kubernetes-service-credential-results
source_filename: azure-kubernetes-service-credential-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CredentialResults\",\n  \"type\": \"object\",\n  \"description\": \"The list of credential result response.\",\n  \"properties\": {\n    \"kubeconfigs\": {\n      \"type\": \"array\",\n      \"description\": \"Base64-encoded Kubernetes configuration file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-credential-results-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: CredentialResults
---
