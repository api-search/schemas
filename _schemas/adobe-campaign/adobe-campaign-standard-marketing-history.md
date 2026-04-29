---
description: MarketingHistory from Adobe Campaign API
layout: schema
name: MarketingHistory
properties_list:
- description: Profile PKEY.
  name: PKey
  type: string
- description: ''
  name: events
  type: array
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-marketing-history-schema.json
slug: adobe-campaign-standard-marketing-history
source_filename: adobe-campaign-standard-marketing-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-marketing-history-schema.json\",\n  \"title\": \"MarketingHistory\",\n  \"description\": \"MarketingHistory from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"Profile PKEY.\",\n      \"example\": \"example_value\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"eventDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Date of the marketing event.\"\n          },\n          \"channel\": {\n            \"type\": \"string\",\n            \"description\": \"Channel of the delivery (email, sms, push).\"\n          },\n          \"deliveryLabel\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Label of the delivery.\"\n          },\n          \"mirrorPage\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"href\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"Link to the mirror page.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-marketing-history-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: MarketingHistory
---
