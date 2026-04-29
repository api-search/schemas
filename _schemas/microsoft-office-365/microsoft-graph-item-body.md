---
description: Represents properties of the body of a message or event.
layout: schema
name: ItemBody
properties_list:
- description: The type of the content. Possible values are text and html.
  name: contentType
  type: string
- description: The content of the item.
  name: content
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-item-body-schema.json
slug: microsoft-graph-item-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemBody\",\n  \"type\": \"object\",\n  \"description\": \"Represents properties of the body of a message or event.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content. Possible values are text and html.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the item.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-item-body-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: ItemBody
---
