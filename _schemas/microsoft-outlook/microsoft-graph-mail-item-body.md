---
description: Represents the body content of a message.
layout: schema
name: ItemBody
properties_list:
- description: The type of the content. Possible values are text and html.
  name: contentType
  type: string
- description: The content of the item body.
  name: content
  type: string
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-item-body-schema.json
slug: microsoft-graph-mail-item-body
source_filename: microsoft-graph-mail-item-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemBody\",\n  \"type\": \"object\",\n  \"description\": \"Represents the body content of a message.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content. Possible values are text and html.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the item body.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-item-body-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: ItemBody
---
