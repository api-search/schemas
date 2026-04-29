---
description: ''
layout: schema
name: AppliedPromotion
properties_list:
- description: ''
  name: promotionId
  type: string
- description: ''
  name: rewards
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-applied-promotion-schema.json
slug: salesforce-applied-promotion
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"promotionId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"rewards\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rewardType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"discountAmount\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"loyaltyProgramCurrencyName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"points\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"relatedInformation\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"notes\": {\n            \"type\": \"string\",\n \
  \           \"example\": \"example_value\"\n          },\n          \"voucherDefinitionName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"voucherExpirationDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"voucherEffectiveDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"loyaltyProgramBadgeName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"memberBadgeStatus\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"badgeValidityEndDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"reason\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"gameDefinitionName\"\
  : {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"rewardType\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"promotionId\",\n    \"rewards\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppliedPromotion\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-applied-promotion-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: AppliedPromotion
---
