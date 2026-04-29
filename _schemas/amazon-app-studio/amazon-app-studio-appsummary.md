---
description: Summary information for an App Studio application.
layout: schema
name: AppSummary
properties_list:
- description: Unique identifier for the application.
  name: appId
  type: string
- description: Display name of the application.
  name: name
  type: string
- description: Current status of the application.
  name: status
  type: string
- description: Creation timestamp.
  name: createdAt
  type: string
provider_name: Amazon App Studio
provider_slug: amazon-app-studio
schema_file: json-schema/amazon-app-studio-appsummary-schema.json
slug: amazon-app-studio-appsummary
source_filename: amazon-app-studio-appsummary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AppSummary\",\n  \"description\": \"Summary information for an App Studio application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the application.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the application.\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-studio/refs/heads/main/json-schema/amazon-app-studio-appsummary-schema.json
tags:
- AWS
- Generative AI
- Internal Tools
- Low-Code
- No-Code
title: AppSummary
---
