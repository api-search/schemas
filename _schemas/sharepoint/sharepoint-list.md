---
description: SharePoint list or document library.
layout: schema
name: List
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Title
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: BaseTemplate
  type: integer
- description: ''
  name: ItemCount
  type: integer
- description: ''
  name: Created
  type: string
- description: ''
  name: LastItemModifiedDate
  type: string
- description: ''
  name: Hidden
  type: boolean
- description: ''
  name: EnableVersioning
  type: boolean
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-list-schema.json
slug: sharepoint-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-schema.json\",\n  \"title\": \"List\",\n  \"description\": \"SharePoint list or document library.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"3fa85f64-5717-4562-b3fc-2c963f66afa6\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"Documents\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"Shared documents library\"\n    },\n    \"BaseTemplate\": {\n      \"type\": \"integer\",\n      \"example\": 101\n    },\n    \"ItemCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"Created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T12:00:00Z\"\n    },\n    \"LastItemModifiedDate\": {\n  \
  \    \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Hidden\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"EnableVersioning\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: List
---
