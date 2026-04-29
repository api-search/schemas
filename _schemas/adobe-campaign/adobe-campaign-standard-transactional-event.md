---
description: TransactionalEvent from Adobe Campaign API
layout: schema
name: TransactionalEvent
properties_list:
- description: Recipient email address (for email channel).
  name: email
  type: string
- description: Recipient mobile phone (for SMS channel).
  name: mobilePhone
  type: string
- description: Push platform (Apple or Google).
  name: pushPlatform
  type: string
- description: Context data for message personalization. Contains dynamic fields matching the transactional message template.
  name: ctx
  type: object
- description: Optional scheduled send time.
  name: scheduled
  type: string
- description: Optional event expiration time.
  name: expiration
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-transactional-event-schema.json
slug: adobe-campaign-standard-transactional-event
source_filename: adobe-campaign-standard-transactional-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-schema.json\",\n  \"title\": \"TransactionalEvent\",\n  \"description\": \"TransactionalEvent from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Recipient email address (for email channel).\",\n      \"example\": \"user@example.com\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient mobile phone (for SMS channel).\",\n      \"example\": \"example_value\"\n    },\n    \"pushPlatform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"apns\",\n        \"gcm\"\n      ],\n      \"description\": \"Push platform (Apple or Google).\",\n      \"example\": \"apns\"\n    },\n    \"ctx\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Context data for message personalization. Contains dynamic fields matching the transactional message template.\",\n      \"additionalProperties\": true\n    },\n    \"scheduled\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Optional scheduled send time.\",\n      \"example\": \"example_value\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Optional event expiration time.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: TransactionalEvent
---
