---
description: Represents a custom application registered in the Productiv platform.
layout: schema
name: Application
properties_list:
- description: The unique identifier for the application.
  name: appId
  type: string
- description: The name of the application.
  name: appName
  type: string
- description: A description of the application.
  name: appDescription
  type: string
- description: The category of the application.
  name: appCategory
  type: string
- description: The URL of the application.
  name: appUrl
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/application.json
slug: application
source_json: "{\n  \"$id\": \"application.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"description\": \"Represents a custom application registered in the Productiv platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"appName\"\n  ],\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the application.\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"appDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the application.\"\n    },\n    \"appCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the application.\"\n    },\n    \"appUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the application.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/application.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: Application
---
