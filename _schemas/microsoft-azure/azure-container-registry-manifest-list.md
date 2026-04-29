---
description: List of manifests.
layout: schema
name: ManifestList
properties_list:
- description: ''
  name: registry
  type: string
- description: ''
  name: imageName
  type: string
- description: ''
  name: manifests
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-manifest-list-schema.json
slug: azure-container-registry-manifest-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManifestList\",\n  \"type\": \"object\",\n  \"description\": \"List of manifests.\",\n  \"properties\": {\n    \"registry\": {\n      \"type\": \"string\"\n    },\n    \"imageName\": {\n      \"type\": \"string\"\n    },\n    \"manifests\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-manifest-list-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManifestList
---
