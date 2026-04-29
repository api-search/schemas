---
description: ''
layout: schema
name: UsedStorage
properties_list:
- description: ''
  name: environmentType
  type: string
- description: ''
  name: environmentName
  type: string
- description: ''
  name: applicationFamily
  type: string
- description: Used database storage in kilobytes
  name: databaseStorageInKilobytes
  type: integer
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-used-storage-schema.json
slug: admin-center-used-storage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsedStorage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentType\": {\n      \"type\": \"string\"\n    },\n    \"environmentName\": {\n      \"type\": \"string\"\n    },\n    \"applicationFamily\": {\n      \"type\": \"string\"\n    },\n    \"databaseStorageInKilobytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Used database storage in kilobytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-used-storage-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: UsedStorage
---
