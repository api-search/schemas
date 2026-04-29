---
description: Recipient information for a message.
layout: schema
name: MessageRecipient
properties_list:
- description: Actor ID of the recipient
  name: actorId
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-message-recipient-schema.json
slug: hubspot-conversations-message-recipient
source_filename: hubspot-conversations-message-recipient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Recipient information for a message.\",\n  \"properties\": {\n    \"actorId\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID of the recipient\",\n      \"example\": \"actor_101\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageRecipient\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-message-recipient-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: MessageRecipient
---
