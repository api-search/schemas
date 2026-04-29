---
description: Description of a restore request.
layout: schema
name: RestoreRequest
properties_list:
- description: RestoreRequest resource specific properties
  name: properties
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-restore-request-schema.json
slug: azure-functions-restore-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-restore-request-schema.json\",\n  \"title\": \"RestoreRequest\",\n  \"description\": \"Description of a restore request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/RestoreRequestProperties\",\n      \"description\": \"RestoreRequest resource specific properties\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-restore-request-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: RestoreRequest
---
