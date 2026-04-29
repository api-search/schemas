---
description: Hybrid Connection contract. This is used to configure a Hybrid Connection.
layout: schema
name: HybridConnection
properties_list:
- description: HybridConnection resource specific properties
  name: properties
  type: object
- description: Kind of resource.
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-hybrid-connection-schema.json
slug: azure-functions-hybrid-connection
source_filename: azure-functions-hybrid-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-hybrid-connection-schema.json\",\n  \"title\": \"HybridConnection\",\n  \"description\": \"Hybrid Connection contract. This is used to configure a Hybrid Connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/HybridConnectionProperties\",\n      \"description\": \"HybridConnection resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-hybrid-connection-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: HybridConnection
---
