---
description: Represents an email address entity.
layout: schema
name: EmailAddress
properties_list:
- description: The display name of the person or entity.
  name: name
  type: string
- description: The email address of the person or entity.
  name: address
  type: string
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-email-address-schema.json
slug: microsoft-graph-mail-email-address
source_filename: microsoft-graph-mail-email-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailAddress\",\n  \"type\": \"object\",\n  \"description\": \"Represents an email address entity.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the person or entity.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the person or entity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-email-address-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: EmailAddress
---
