---
description: Resource group information for update.
layout: schema
name: ResourceGroupPatchable
properties_list:
- description: The name of the resource group.
  name: name
  type: string
- description: The tags attached to the resource group.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-resource-group-patchable-schema.json
slug: azure-resource-manager-resource-group-patchable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceGroupPatchable\",\n  \"type\": \"object\",\n  \"description\": \"Resource group information for update.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource group.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags attached to the resource group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-resource-group-patchable-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ResourceGroupPatchable
---
