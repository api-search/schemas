---
description: CreditsResponse schema from ActiveCampaign API
layout: schema
name: CreditsResponse
properties_list:
- description: ''
  name: smsCredits
  type: object
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-credits-response-schema.json
slug: activecampaign-sms-credits-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-credits-response-schema.json\",\n  \"title\": \"CreditsResponse\",\n  \"description\": \"CreditsResponse schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"smsCredits\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"period\": {\n          \"type\": \"string\",\n          \"example\": \"month\"\n        },\n        \"nextRefillDate\": {\n          \"type\": \"string\",\n          \"example\": \"2026-02-26 15:06:25\"\n        },\n        \"includedThisPeriod\": {\n          \"type\": \"integer\",\n          \"example\": 1000\n        },\n        \"usedThisPeriod\": {\n          \"type\": \"integer\",\n          \"example\": 71\n        },\n        \"extra\": {\n          \"type\": \"integer\",\n          \"example\": 9040\n      \
  \  },\n        \"available\": {\n          \"type\": \"integer\",\n          \"example\": 9969\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-credits-response-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: CreditsResponse
---
