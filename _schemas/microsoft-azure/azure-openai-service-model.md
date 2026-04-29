---
description: Describes an OpenAI model.
layout: schema
name: Model
properties_list:
- description: The model identifier.
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: The Unix timestamp when the model was created.
  name: created
  type: integer
- description: The organization that owns the model.
  name: owned_by
  type: string
- description: The capabilities of the model.
  name: capabilities
  type: object
- description: The lifecycle status of the model.
  name: lifecycle_status
  type: string
- description: Deprecation information for the model.
  name: deprecation
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-model-schema.json
slug: azure-openai-service-model
source_filename: azure-openai-service-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Model\",\n  \"type\": \"object\",\n  \"description\": \"Describes an OpenAI model.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The model identifier.\"\n    },\n    \"object\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp when the model was created.\"\n    },\n    \"owned_by\": {\n      \"type\": \"string\",\n      \"description\": \"The organization that owns the model.\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"The capabilities of the model.\"\n    },\n    \"lifecycle_status\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle status of the model.\"\n    },\n    \"deprecation\": {\n      \"type\": \"object\",\n      \"description\": \"Deprecation information for the model.\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-model-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Model
---
