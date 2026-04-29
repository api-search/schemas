---
description: String dictionary resource.
layout: schema
name: StringDictionary
properties_list:
- description: Settings.
  name: properties
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-string-dictionary-schema.json
slug: azure-functions-string-dictionary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-string-dictionary-schema.json\",\n  \"title\": \"StringDictionary\",\n  \"description\": \"String dictionary resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Settings.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-string-dictionary-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: StringDictionary
---
