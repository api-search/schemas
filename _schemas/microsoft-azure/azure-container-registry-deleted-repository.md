---
description: Deleted repository result.
layout: schema
name: DeletedRepository
properties_list:
- description: Digests of manifests deleted.
  name: manifestsDeleted
  type: array
- description: Tags deleted.
  name: tagsDeleted
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-deleted-repository-schema.json
slug: azure-container-registry-deleted-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedRepository\",\n  \"type\": \"object\",\n  \"description\": \"Deleted repository result.\",\n  \"properties\": {\n    \"manifestsDeleted\": {\n      \"type\": \"array\",\n      \"description\": \"Digests of manifests deleted.\"\n    },\n    \"tagsDeleted\": {\n      \"type\": \"array\",\n      \"description\": \"Tags deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-deleted-repository-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeletedRepository
---
