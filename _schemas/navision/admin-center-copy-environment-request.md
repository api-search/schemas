---
description: ''
layout: schema
name: CopyEnvironmentRequest
properties_list:
- description: Name for the new environment
  name: environmentName
  type: string
- description: Type of environment to create
  name: type
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-copy-environment-request-schema.json
slug: admin-center-copy-environment-request
source_filename: admin-center-copy-environment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopyEnvironmentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new environment\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of environment to create\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-copy-environment-request-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: CopyEnvironmentRequest
---
