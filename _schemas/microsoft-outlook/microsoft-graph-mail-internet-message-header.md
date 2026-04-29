---
description: A key-value pair representing an Internet message header as defined by RFC 5322.
layout: schema
name: InternetMessageHeader
properties_list:
- description: The name of the message header.
  name: name
  type: string
- description: The value of the message header.
  name: value
  type: string
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-internet-message-header-schema.json
slug: microsoft-graph-mail-internet-message-header
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InternetMessageHeader\",\n  \"type\": \"object\",\n  \"description\": \"A key-value pair representing an Internet message header as defined by RFC 5322.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the message header.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the message header.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-internet-message-header-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: InternetMessageHeader
---
