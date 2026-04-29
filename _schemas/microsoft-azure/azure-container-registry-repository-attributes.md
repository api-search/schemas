---
description: Repository attributes.
layout: schema
name: RepositoryAttributes
properties_list:
- description: Registry name.
  name: registry
  type: string
- description: Image name.
  name: imageName
  type: string
- description: Image created time.
  name: createdTime
  type: string
- description: Image last update time.
  name: lastUpdateTime
  type: string
- description: Number of manifests.
  name: manifestCount
  type: integer
- description: Number of tags.
  name: tagCount
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-repository-attributes-schema.json
slug: azure-container-registry-repository-attributes
source_filename: azure-container-registry-repository-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepositoryAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Repository attributes.\",\n  \"properties\": {\n    \"registry\": {\n      \"type\": \"string\",\n      \"description\": \"Registry name.\"\n    },\n    \"imageName\": {\n      \"type\": \"string\",\n      \"description\": \"Image name.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"description\": \"Image created time.\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Image last update time.\"\n    },\n    \"manifestCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of manifests.\"\n    },\n    \"tagCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-repository-attributes-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: RepositoryAttributes
---
