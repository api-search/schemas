---
description: Entity representing the reference to the deployment parameters.
layout: schema
name: ParametersLink
properties_list:
- description: The URI of the parameters file.
  name: uri
  type: string
- description: The content version of the parameters.
  name: contentVersion
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-parameters-link-schema.json
slug: azure-resource-manager-parameters-link
source_filename: azure-resource-manager-parameters-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParametersLink\",\n  \"type\": \"object\",\n  \"description\": \"Entity representing the reference to the deployment parameters.\",\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI of the parameters file.\"\n    },\n    \"contentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The content version of the parameters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-parameters-link-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ParametersLink
---
