---
description: Delivery status information for a message
layout: schema
name: MessageStatus
properties_list:
- description: Current delivery status type
  name: statusType
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-message-status-schema.json
slug: hubspot-conversations-message-status
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Delivery status information for a message\",\n  \"properties\": {\n    \"statusType\": {\n      \"type\": \"string\",\n      \"description\": \"Current delivery status type\",\n      \"example\": \"DELIVERED\",\n      \"enum\": [\n        \"SENT\",\n        \"DELIVERED\",\n        \"READ\",\n        \"FAILED\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-message-status-schema.json
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
title: MessageStatus
---
