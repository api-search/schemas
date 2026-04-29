---
description: ''
layout: schema
name: FolderInput
properties_list:
- description: The title of the Folder.
  name: title
  type: string
- description: The token of the parent Folder for nesting.
  name: parent_folder_token
  type: string
- description: The token of the Workspace for the Folder.
  name: workspace_token
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-folder-input-schema.json
slug: vantage-cost-management-folder-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FolderInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Folder.\"\n    },\n    \"parent_folder_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the parent Folder for nesting.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the Folder.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-folder-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: FolderInput
---
