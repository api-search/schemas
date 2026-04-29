---
description: ''
layout: schema
name: EligibleLoyaltyTier
properties_list:
- description: ''
  name: tierGroup
  type: object
- description: ''
  name: tier
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-eligible-loyalty-tier-schema.json
slug: salesforce-eligible-loyalty-tier
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"tierGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"id\"\n      ]\n    },\n    \"tier\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"id\"\n      ]\n    }\n  },\n  \"required\": [\n    \"tierGroup\",\n    \"tier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EligibleLoyaltyTier\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-eligible-loyalty-tier-schema.json
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
title: EligibleLoyaltyTier
---
