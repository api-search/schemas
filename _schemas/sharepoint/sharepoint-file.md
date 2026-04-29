---
description: SharePoint file.
layout: schema
name: File
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: ServerRelativeUrl
  type: string
- description: ''
  name: Length
  type: integer
- description: ''
  name: TimeCreated
  type: string
- description: ''
  name: TimeLastModified
  type: string
- description: ''
  name: CheckOutType
  type: integer
- description: ''
  name: MajorVersion
  type: integer
- description: ''
  name: MinorVersion
  type: integer
- description: ''
  name: UniqueId
  type: string
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-file-schema.json
slug: sharepoint-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-file-schema.json\",\n  \"title\": \"File\",\n  \"description\": \"SharePoint file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"report.pdf\"\n    },\n    \"ServerRelativeUrl\": {\n      \"type\": \"string\",\n      \"example\": \"/sites/mysite/Shared Documents/report.pdf\"\n    },\n    \"Length\": {\n      \"type\": \"integer\",\n      \"example\": 1048576\n    },\n    \"TimeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T09:00:00Z\"\n    },\n    \"TimeLastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T10:30:00Z\"\n    },\n    \"CheckOutType\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    },\n\
  \    \"MajorVersion\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"MinorVersion\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"UniqueId\": {\n      \"type\": \"string\",\n      \"example\": \"3fa85f64-5717-4562-b3fc-2c963f66afa6\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-file-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: File
---
