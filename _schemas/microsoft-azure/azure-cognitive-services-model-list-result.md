---
description: The list of cognitive services models.
layout: schema
name: ModelListResult
properties_list:
- description: An array of models.
  name: value
  type: array
- description: The link used to get the next page of models.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-model-list-result-schema.json
slug: azure-cognitive-services-model-list-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelListResult\",\n  \"type\": \"object\",\n  \"description\": \"The list of cognitive services models.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"An array of models.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The link used to get the next page of models.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-model-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ModelListResult
---
