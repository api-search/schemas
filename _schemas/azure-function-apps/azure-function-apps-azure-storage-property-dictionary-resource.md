---
description: AzureStorageInfo dictionary resource.
layout: schema
name: AzureStoragePropertyDictionaryResource
properties_list:
- description: Azure storage accounts.
  name: properties
  type: object
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-azure-storage-property-dictionary-resource-schema.json
slug: azure-function-apps-azure-storage-property-dictionary-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-azure-storage-property-dictionary-resource-schema.json\",\n  \"title\": \"AzureStoragePropertyDictionaryResource\",\n  \"description\": \"AzureStorageInfo dictionary resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/AzureStorageInfoValue\"\n      },\n      \"description\": \"Azure storage accounts.\",\n      \"type\": \"object\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-azure-storage-property-dictionary-resource-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: AzureStoragePropertyDictionaryResource
---
