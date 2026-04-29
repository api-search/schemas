---
description: Represents a single application with a limited set of attributes from the Productiv portfolio.
layout: schema
name: AppSummary
properties_list:
- description: The unique identifier of the application.
  name: ApplicationId
  type: string
- description: The name of the application.
  name: AppName
  type: string
- description: The current status of the application.
  name: AppStatus
  type: string
- description: The name of the vendor.
  name: VendorName
  type: string
- description: The category of the application.
  name: AppCategory
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/app-summary.json
slug: app-summary
source_filename: app-summary.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"app-summary.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppSummary\",\n  \"description\": \"Represents a single application with a limited set of attributes from the Productiv portfolio.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application.\"\n    },\n    \"AppName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"AppStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application.\"\n    },\n    \"VendorName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the vendor.\"\n    },\n    \"AppCategory\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the application.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/app-summary.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: AppSummary
---
