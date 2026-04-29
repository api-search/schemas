---
description: AIBroadcastUpdateRequest schema from ActiveCampaign API
layout: schema
name: AIBroadcastUpdateRequest
properties_list:
- description: ''
  name: source
  type: string
- description: ''
  name: prompt
  type: string
- description: ''
  name: tone
  type: string
- description: ''
  name: broadcastId
  type: integer
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-ai-broadcast-update-request-schema.json
slug: activecampaign-sms-ai-broadcast-update-request
source_filename: activecampaign-sms-ai-broadcast-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-update-request-schema.json\",\n  \"title\": \"AIBroadcastUpdateRequest\",\n  \"description\": \"AIBroadcastUpdateRequest schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ai_index\",\n        \"sms_index\",\n        \"ai_builder\"\n      ]\n    },\n    \"prompt\": {\n      \"type\": \"string\"\n    },\n    \"tone\": {\n      \"type\": \"string\"\n    },\n    \"broadcastId\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"prompt\",\n    \"tone\",\n    \"broadcastId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-update-request-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: AIBroadcastUpdateRequest
---
