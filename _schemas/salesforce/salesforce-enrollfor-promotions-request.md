---
description: ''
layout: schema
name: EnrollforPromotionsRequest
properties_list:
- description: ''
  name: processParameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-enrollfor-promotions-request-schema.json
slug: salesforce-enrollfor-promotions-request
source_filename: salesforce-enrollfor-promotions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"processParameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"MembershipNumber\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"PromotionId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"MembershipNumber\",\n          \"PromotionId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"processParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnrollforPromotionsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-enrollfor-promotions-request-schema.json
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
title: EnrollforPromotionsRequest
---
