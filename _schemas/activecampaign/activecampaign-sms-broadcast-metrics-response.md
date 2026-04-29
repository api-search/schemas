---
description: BroadcastMetricsResponse schema from ActiveCampaign API
layout: schema
name: BroadcastMetricsResponse
properties_list:
- description: ''
  name: metrics
  type: array
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-broadcast-metrics-response-schema.json
slug: activecampaign-sms-broadcast-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-metrics-response-schema.json\",\n  \"title\": \"BroadcastMetricsResponse\",\n  \"description\": \"BroadcastMetricsResponse schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BroadcastMetrics\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-metrics-response-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: BroadcastMetricsResponse
---
