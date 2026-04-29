---
description: Entity representing the reference to the template.
layout: schema
name: TemplateLink
properties_list:
- description: The URI of the template.
  name: uri
  type: string
- description: The content version of the template.
  name: contentVersion
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-template-link-schema.json
slug: azure-resource-manager-template-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplateLink\",\n  \"type\": \"object\",\n  \"description\": \"Entity representing the reference to the template.\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI of the template.\"\n    },\n    \"contentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The content version of the template.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-template-link-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: TemplateLink
---
