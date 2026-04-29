---
description: Options for app content migration.
layout: schema
name: StorageMigrationOptions
properties_list:
- description: StorageMigrationOptions resource specific properties
  name: properties
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-storage-migration-options-schema.json
slug: azure-functions-storage-migration-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-storage-migration-options-schema.json\",\n  \"title\": \"StorageMigrationOptions\",\n  \"description\": \"Options for app content migration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/StorageMigrationOptionsProperties\",\n      \"description\": \"StorageMigrationOptions resource specific properties\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-storage-migration-options-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: StorageMigrationOptions
---
