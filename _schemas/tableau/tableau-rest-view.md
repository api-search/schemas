---
description: ''
layout: schema
name: View
properties_list:
- description: The unique identifier for the view.
  name: id
  type: string
- description: The name of the view.
  name: name
  type: string
- description: The URL name of the view.
  name: contentUrl
  type: string
- description: The date and time the view was created.
  name: createdAt
  type: string
- description: The date and time the view was last updated.
  name: updatedAt
  type: string
- description: The URL-friendly name of the view used in the content URL.
  name: viewUrlName
  type: string
- description: The type of sheet (worksheet, dashboard, or story).
  name: sheetType
  type: string
- description: ''
  name: project
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: workbook
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: usage
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-view-schema.json
slug: tableau-rest-view
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"View\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the view.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the view.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL name of the view.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the view was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the view was last updated.\"\n    },\n    \"viewUrlName\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly name of the view used in the content URL.\"\n    },\n    \"sheetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of sheet (worksheet, dashboard,\
  \ or story).\"\n    },\n    \"project\": {\n      \"type\": \"object\"\n    },\n    \"owner\": {\n      \"type\": \"object\"\n    },\n    \"workbook\": {\n      \"type\": \"object\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-view-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: View
---
