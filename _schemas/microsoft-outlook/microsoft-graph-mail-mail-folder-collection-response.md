---
description: Collection of mail folder resources with optional pagination link.
layout: schema
name: MailFolderCollectionResponse
properties_list:
- description: ''
  name: '@odata.context'
  type: string
- description: ''
  name: '@odata.nextLink'
  type: string
- description: ''
  name: value
  type: array
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-mail-folder-collection-response-schema.json
slug: microsoft-graph-mail-mail-folder-collection-response
source_filename: microsoft-graph-mail-mail-folder-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MailFolderCollectionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Collection of mail folder resources with optional pagination link.\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-mail-folder-collection-response-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: MailFolderCollectionResponse
---
