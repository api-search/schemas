---
description: ListItemCreateRequest from SharePoint API
layout: schema
name: ListItemCreateRequest
properties_list:
- description: ''
  name: __metadata
  type: object
- description: ''
  name: Title
  type: string
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-list-item-create-request-schema.json
slug: sharepoint-list-item-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-item-create-request-schema.json\",\n  \"title\": \"ListItemCreateRequest\",\n  \"description\": \"ListItemCreateRequest from SharePoint API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"SP.Data.MyListListItem\"\n        }\n      }\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"New Item\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-item-create-request-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: ListItemCreateRequest
---
