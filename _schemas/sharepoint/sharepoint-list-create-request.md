---
description: Request to create a new SharePoint list.
layout: schema
name: ListCreateRequest
properties_list:
- description: ''
  name: __metadata
  type: object
- description: ''
  name: Title
  type: string
- description: ''
  name: Description
  type: string
- description: 100=Generic List, 101=Document Library, 104=Announcements
  name: BaseTemplate
  type: integer
- description: ''
  name: AllowContentTypes
  type: boolean
- description: ''
  name: ContentTypesEnabled
  type: boolean
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-list-create-request-schema.json
slug: sharepoint-list-create-request
source_filename: sharepoint-list-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-create-request-schema.json\",\n  \"title\": \"ListCreateRequest\",\n  \"description\": \"Request to create a new SharePoint list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"SP.List\"\n        }\n      }\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"My New List\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"A custom list\"\n    },\n    \"BaseTemplate\": {\n      \"type\": \"integer\",\n      \"example\": 100,\n      \"description\": \"100=Generic List, 101=Document Library, 104=Announcements\"\n    },\n    \"AllowContentTypes\": {\n      \"type\": \"boolean\",\n  \
  \    \"example\": true\n    },\n    \"ContentTypesEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"Title\",\n    \"BaseTemplate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-list-create-request-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: ListCreateRequest
---
