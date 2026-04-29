---
description: List of repositories.
layout: schema
name: Repositories
properties_list:
- description: List of repository names.
  name: repositories
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-repositories-schema.json
slug: azure-container-registry-repositories
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Repositories\",\n  \"type\": \"object\",\n  \"description\": \"List of repositories.\",\n  \"properties\": {\n    \"repositories\": {\n      \"type\": \"array\",\n      \"description\": \"List of repository names.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-repositories-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Repositories
---
