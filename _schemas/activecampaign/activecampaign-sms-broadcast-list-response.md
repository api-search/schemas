---
description: BroadcastListResponse schema from ActiveCampaign API
layout: schema
name: BroadcastListResponse
properties_list:
- description: ''
  name: broadcasts
  type: array
- description: ''
  name: meta
  type: object
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-broadcast-list-response-schema.json
slug: activecampaign-sms-broadcast-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-list-response-schema.json\",\n  \"title\": \"BroadcastListResponse\",\n  \"description\": \"BroadcastListResponse schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"broadcasts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BroadcastMessage\"\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"total\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of broadcasts\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-list-response-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: BroadcastListResponse
---
