---
description: Represents a completion response from the API.
layout: schema
name: CreateCompletionResponse
properties_list:
- description: A unique identifier for the completion.
  name: id
  type: string
- description: The object type.
  name: object
  type: string
- description: The Unix timestamp of when the completion was created.
  name: created
  type: integer
- description: The model used for completion.
  name: model
  type: string
- description: The list of completion choices.
  name: choices
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-completion-response-schema.json
slug: azure-openai-service-create-completion-response
source_filename: azure-openai-service-create-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCompletionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Represents a completion response from the API.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the completion.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp of when the completion was created.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for completion.\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"The list of completion choices.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-completion-response-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateCompletionResponse
---
