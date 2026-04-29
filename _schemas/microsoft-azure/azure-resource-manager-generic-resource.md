---
description: Resource information.
layout: schema
name: GenericResource
properties_list:
- description: The resource properties.
  name: properties
  type: object
- description: The kind of the resource.
  name: kind
  type: string
- description: ID of the resource that manages this resource.
  name: managedBy
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-generic-resource-schema.json
slug: azure-resource-manager-generic-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenericResource\",\n  \"type\": \"object\",\n  \"description\": \"Resource information.\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The resource properties.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of the resource.\"\n    },\n    \"managedBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the resource that manages this resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-generic-resource-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: GenericResource
---
