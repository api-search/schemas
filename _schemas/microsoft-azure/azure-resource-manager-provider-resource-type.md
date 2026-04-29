---
description: Resource type managed by the resource provider.
layout: schema
name: ProviderResourceType
properties_list:
- description: The resource type.
  name: resourceType
  type: string
- description: The collection of locations where this resource type can be created.
  name: locations
  type: array
- description: The API version.
  name: apiVersions
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-provider-resource-type-schema.json
slug: azure-resource-manager-provider-resource-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProviderResourceType\",\n  \"type\": \"object\",\n  \"description\": \"Resource type managed by the resource provider.\",\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of locations where this resource type can be created.\"\n    },\n    \"apiVersions\": {\n      \"type\": \"array\",\n      \"description\": \"The API version.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-provider-resource-type-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ProviderResourceType
---
