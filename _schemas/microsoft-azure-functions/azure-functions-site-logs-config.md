---
description: Configuration of App Service site logs.
layout: schema
name: SiteLogsConfig
properties_list:
- description: SiteLogsConfig resource specific properties
  name: properties
  type: object
- description: Kind of resource.
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-site-logs-config-schema.json
slug: azure-functions-site-logs-config
source_filename: azure-functions-site-logs-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-logs-config-schema.json\",\n  \"title\": \"SiteLogsConfig\",\n  \"description\": \"Configuration of App Service site logs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/SiteLogsConfigProperties\",\n      \"description\": \"SiteLogsConfig resource specific properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-logs-config-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: SiteLogsConfig
---
