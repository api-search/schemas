---
description: Usage statistics for the API call.
layout: schema
name: Usage
properties_list:
- description: Number of tokens in the prompt.
  name: prompt_tokens
  type: integer
- description: Number of tokens in the generated completion.
  name: completion_tokens
  type: integer
- description: Total number of tokens used in the request.
  name: total_tokens
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-usage-schema.json
slug: azure-openai-service-usage
source_filename: azure-openai-service-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage\",\n  \"type\": \"object\",\n  \"description\": \"Usage statistics for the API call.\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the prompt.\"\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the generated completion.\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of tokens used in the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-usage-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Usage
---
