---
description: ''
layout: schema
name: EnvironmentSettings
properties_list:
- description: Application Insights instrumentation key
  name: appInsightsKey
  type: string
- description: ''
  name: updateWindow
  type: object
- description: Security group assigned to the environment
  name: securityGroupId
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/admin-center-environment-settings-schema.json
slug: admin-center-environment-settings
source_filename: admin-center-environment-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appInsightsKey\": {\n      \"type\": \"string\",\n      \"description\": \"Application Insights instrumentation key\"\n    },\n    \"updateWindow\": {\n      \"type\": \"object\"\n    },\n    \"securityGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"Security group assigned to the environment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/admin-center-environment-settings-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: EnvironmentSettings
---
