---
description: An Amazon App Studio application.
layout: schema
name: App
properties_list:
- description: Unique identifier for the application.
  name: appId
  type: string
- description: Display name of the application.
  name: name
  type: string
- description: Description of the application purpose.
  name: description
  type: string
- description: Current status of the application.
  name: status
  type: string
- description: Timestamp when the application was created.
  name: createdAt
  type: string
- description: Timestamp when the application was last updated.
  name: updatedAt
  type: string
provider_name: Amazon App Studio
provider_slug: amazon-app-studio
schema_file: json-schema/amazon-app-studio-app-schema.json
slug: amazon-app-studio-app
source_filename: amazon-app-studio-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"App\",\n  \"description\": \"An Amazon App Studio application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application purpose.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the application.\",\n      \"enum\": [\n        \"CREATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was created.\"\n    },\n    \"updatedAt\": {\n      \"\
  type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-studio/refs/heads/main/json-schema/amazon-app-studio-app-schema.json
tags:
- AWS
- Generative AI
- Internal Tools
- Low-Code
- No-Code
title: App
---
