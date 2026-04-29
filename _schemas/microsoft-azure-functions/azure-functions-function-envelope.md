---
description: Function information.
layout: schema
name: FunctionEnvelope
properties_list:
- description: FunctionEnvelope resource specific properties
  name: properties
  type: object
- description: Kind of resource.
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-function-envelope-schema.json
slug: azure-functions-function-envelope
source_filename: azure-functions-function-envelope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-function-envelope-schema.json\",\n  \"title\": \"FunctionEnvelope\",\n  \"description\": \"Function information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/FunctionEnvelopeProperties\",\n      \"description\": \"FunctionEnvelope resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-function-envelope-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: FunctionEnvelope
---
