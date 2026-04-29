---
description: AIBroadcastRequest schema from ActiveCampaign API
layout: schema
name: AIBroadcastRequest
properties_list:
- description: ''
  name: source
  type: string
- description: User prompt for AI generation
  name: prompt
  type: string
- description: Desired tone for the message
  name: tone
  type: string
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-ai-broadcast-request-schema.json
slug: activecampaign-sms-ai-broadcast-request
source_filename: activecampaign-sms-ai-broadcast-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-request-schema.json\",\n  \"title\": \"AIBroadcastRequest\",\n  \"description\": \"AIBroadcastRequest schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ai_index\",\n        \"sms_index\",\n        \"ai_builder\"\n      ]\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"User prompt for AI generation\"\n    },\n    \"tone\": {\n      \"type\": \"string\",\n      \"description\": \"Desired tone for the message\"\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"prompt\",\n    \"tone\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-request-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: AIBroadcastRequest
---
