---
description: Configuration settings for the Azure App Service Authentication / Authorization feature.
layout: schema
name: SiteAuthSettings
properties_list:
- description: SiteAuthSettings resource specific properties
  name: properties
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-site-auth-settings-schema.json
slug: azure-functions-site-auth-settings
source_filename: azure-functions-site-auth-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-auth-settings-schema.json\",\n  \"title\": \"SiteAuthSettings\",\n  \"description\": \"Configuration settings for the Azure App Service Authentication / Authorization feature.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/SiteAuthSettingsProperties\",\n      \"description\": \"SiteAuthSettings resource specific properties\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-site-auth-settings-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: SiteAuthSettings
---
