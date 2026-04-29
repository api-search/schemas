---
description: Cognitive Services account model.
layout: schema
name: AccountModel
properties_list:
- description: Model format.
  name: format
  type: string
- description: Model name.
  name: name
  type: string
- description: Model version.
  name: version
  type: string
- description: Source of the model.
  name: source
  type: string
- description: The maximum capacity.
  name: maxCapacity
  type: integer
- description: Model capabilities.
  name: capabilities
  type: object
- description: Deprecation information.
  name: deprecation
  type: object
- description: Model lifecycle status.
  name: lifecycleStatus
  type: string
- description: ''
  name: systemData
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-account-model-schema.json
slug: azure-cognitive-services-account-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountModel\",\n  \"type\": \"object\",\n  \"description\": \"Cognitive Services account model.\",\n  \"properties\": {\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Model format.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Model name.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Model version.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the model.\"\n    },\n    \"maxCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum capacity.\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"Model capabilities.\"\n    },\n    \"deprecation\": {\n      \"type\": \"object\",\n      \"description\": \"Deprecation information.\"\n    },\n    \"lifecycleStatus\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Model lifecycle status.\"\n    },\n    \"systemData\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-account-model-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AccountModel
---
