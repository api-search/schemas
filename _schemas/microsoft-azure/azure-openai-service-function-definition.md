---
description: The function definition.
layout: schema
name: FunctionDefinition
properties_list:
- description: The name of the function to be called.
  name: name
  type: string
- description: A description of what the function does.
  name: description
  type: string
- description: The parameters the functions accepts, described as a JSON Schema object.
  name: parameters
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-function-definition-schema.json
slug: azure-openai-service-function-definition
source_filename: azure-openai-service-function-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionDefinition\",\n  \"type\": \"object\",\n  \"description\": \"The function definition.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function to be called.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the function does.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"The parameters the functions accepts, described as a JSON Schema object.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-function-definition-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: FunctionDefinition
---
