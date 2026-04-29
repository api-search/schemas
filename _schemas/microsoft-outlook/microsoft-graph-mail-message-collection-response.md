---
description: Collection of message resources with optional pagination link.
layout: schema
name: MessageCollectionResponse
properties_list:
- description: The OData context URL.
  name: '@odata.context'
  type: string
- description: The total count of matching resources.
  name: '@odata.count'
  type: integer
- description: The URL for the next page of results.
  name: '@odata.nextLink'
  type: string
- description: ''
  name: value
  type: array
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-message-collection-response-schema.json
slug: microsoft-graph-mail-message-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageCollectionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Collection of message resources with optional pagination link.\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\",\n      \"description\": \"The OData context URL.\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total count of matching resources.\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the next page of results.\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-message-collection-response-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: MessageCollectionResponse
---
