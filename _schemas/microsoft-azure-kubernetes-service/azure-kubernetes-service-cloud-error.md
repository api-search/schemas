---
description: An error response from the Container service.
layout: schema
name: CloudError
properties_list:
- description: Details about the error.
  name: error
  type: object
provider_name: Azure Kubernetes Service
provider_slug: microsoft-azure-kubernetes-service
schema_file: json-schema/azure-kubernetes-service-cloud-error-schema.json
slug: azure-kubernetes-service-cloud-error
source_filename: azure-kubernetes-service-cloud-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CloudError\",\n  \"type\": \"object\",\n  \"description\": \"An error response from the Container service.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-kubernetes-service/refs/heads/main/json-schema/azure-kubernetes-service-cloud-error-schema.json
tags:
- Azure
- Cloud
- Containers
- DevOps
- Kubernetes
- Orchestration
title: CloudError
---
