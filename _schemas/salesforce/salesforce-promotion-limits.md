---
description: ''
layout: schema
name: PromotionLimits
properties_list:
- description: ''
  name: perLineItemLimit
  type: integer
- description: ''
  name: vouchersLimit
  type: integer
- description: ''
  name: vouchersPerCustomerLimit
  type: integer
- description: ''
  name: perCartLimit
  type: integer
- description: ''
  name: usePerCustomerLimit
  type: integer
- description: ''
  name: liabilityLimit
  type: integer
- description: ''
  name: loyaltyProgramCurrency
  type: object
- description: ''
  name: pointsPerCustomerLimit
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-promotion-limits-schema.json
slug: salesforce-promotion-limits
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"perLineItemLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"vouchersLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"vouchersPerCustomerLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"perCartLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"usePerCustomerLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"liabilityLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"loyaltyProgramCurrency\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"pointsPerCustomerLimit\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"perLineItemLimit\"\
  ,\n    \"vouchersLimit\",\n    \"vouchersPerCustomerLimit\",\n    \"perCartLimit\",\n    \"usePerCustomerLimit\",\n    \"liabilityLimit\",\n    \"loyaltyProgramCurrency\",\n    \"pointsPerCustomerLimit\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PromotionLimits\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-promotion-limits-schema.json
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
title: PromotionLimits
---
