---
description: SharePoint site (web) properties.
layout: schema
name: Web
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
  name: Url
  type: string
- description: ''
  name: WebTemplate
  type: string
- description: ''
  name: Created
  type: string
- description: ''
  name: LastItemModifiedDate
  type: string
- description: ''
  name: Language
  type: integer
- description: ''
  name: ServerRelativeUrl
  type: string
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-web-schema.json
slug: sharepoint-web
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-web-schema.json\",\n  \"title\": \"Web\",\n  \"description\": \"SharePoint site (web) properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"3fa85f64-5717-4562-b3fc-2c963f66afa6\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"My SharePoint Site\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"Team collaboration site\"\n    },\n    \"Url\": {\n      \"type\": \"string\",\n      \"example\": \"https://contoso.sharepoint.com/sites/mysite\"\n    },\n    \"WebTemplate\": {\n      \"type\": \"string\",\n      \"example\": \"STS\"\n    },\n    \"Created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2024-01-15T12:00:00Z\"\n\
  \    },\n    \"LastItemModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T08:30:00Z\"\n    },\n    \"Language\": {\n      \"type\": \"integer\",\n      \"example\": 1033\n    },\n    \"ServerRelativeUrl\": {\n      \"type\": \"string\",\n      \"example\": \"/sites/mysite\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-web-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: Web
---
