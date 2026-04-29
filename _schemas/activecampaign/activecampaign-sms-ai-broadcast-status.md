---
description: AIBroadcastStatus schema from ActiveCampaign API
layout: schema
name: AIBroadcastStatus
properties_list:
- description: ''
  name: source
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: broadcastId
  type: integer
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-ai-broadcast-status-schema.json
slug: activecampaign-sms-ai-broadcast-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-status-schema.json\",\n  \"title\": \"AIBroadcastStatus\",\n  \"description\": \"AIBroadcastStatus schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ai_index\",\n        \"sms_index\",\n        \"ai_builder\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"in_progress\",\n        \"error\",\n        \"success\"\n      ]\n    },\n    \"broadcastId\": {\n      \"type\": \"integer\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-ai-broadcast-status-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: AIBroadcastStatus
---
