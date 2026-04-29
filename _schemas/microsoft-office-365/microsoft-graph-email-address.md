---
description: The name and email address of a contact or message recipient.
layout: schema
name: EmailAddress
properties_list:
- description: The display name of the person or entity.
  name: name
  type: string
- description: The email address of the person or entity.
  name: address
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-email-address-schema.json
slug: microsoft-graph-email-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailAddress\",\n  \"type\": \"object\",\n  \"description\": \"The name and email address of a contact or message recipient.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the person or entity.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the person or entity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-email-address-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: EmailAddress
---
