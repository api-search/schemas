---
description: A Folder for organizing Cost Reports within a Workspace, supporting nested folder hierarchies.
layout: schema
name: Vantage Folder
properties_list:
- description: The unique token identifier for the Folder.
  name: token
  type: string
- description: The title of the Folder.
  name: title
  type: string
- description: The token of the parent Folder, if nested.
  name: parent_folder_token
  type: string
- description: The token of the Workspace this Folder belongs to.
  name: workspace_token
  type: string
- description: The date and time the Folder was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/folder.json
slug: folder
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/folder.json\",\n  \"title\": \"Vantage Folder\",\n  \"description\": \"A Folder for organizing Cost Reports within a Workspace, supporting nested folder hierarchies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Folder.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Folder.\"\n    },\n    \"parent_folder_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the parent Folder, if nested.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this Folder belongs to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The date and time the Folder was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/folder.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Folder
---
