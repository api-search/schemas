---
description: ''
layout: schema
name: CreateEnvironmentRequest
properties_list:
- description: Type of environment to create
  name: environmentType
  type: string
- description: Country to create the environment within
  name: countryCode
  type: string
- description: Logical ring group (only Sandbox may be created in Preview ring)
  name: ringName
  type: string
- description: Application version (e.g., 26.0.0.0)
  name: applicationVersion
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-create-environment-request-schema.json
slug: admin-center-create-environment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEnvironmentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of environment to create\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country to create the environment within\"\n    },\n    \"ringName\": {\n      \"type\": \"string\",\n      \"description\": \"Logical ring group (only Sandbox may be created in Preview ring)\"\n    },\n    \"applicationVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Application version (e.g., 26.0.0.0)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-create-environment-request-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: CreateEnvironmentRequest
---
