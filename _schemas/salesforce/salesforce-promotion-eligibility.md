---
description: ''
layout: schema
name: PromotionEligibility
properties_list:
- description: ''
  name: eligibleProductCategories
  type: array
- description: ''
  name: eligibleProducts
  type: array
- description: ''
  name: eligibleChannels
  type: array
- description: ''
  name: eligibleCustomerEvents
  type: object
- description: ''
  name: eligibleEnrollmentPeriod
  type: object
- description: ''
  name: eligibleLoyaltyTiers
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-promotion-eligibility-schema.json
slug: salesforce-promotion-eligibility
source_filename: salesforce-promotion-eligibility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"eligibleProductCategories\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    },\n    \"eligibleProducts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"name\"\n        ]\n      }\n    },\n    \"eligibleChannels\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n\
  \        \"properties\": {\n          \"channelType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"store\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          },\n          \"retailLocationGroup\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"required\": [\n          \"channelType\",\n          \"store\",\n          \"retailLocationGroup\"\n        ]\n      }\n    },\n    \"eligibleCustomerEvents\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"event\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"eventPeriodUnit\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"event\",\n        \"eventPeriodUnit\"\n      ]\n    },\n    \"eligibleEnrollmentPeriod\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isEnrollmentRequired\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"enrollmentStartDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"enrollmentEndDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"isEnrollmentRequired\",\n        \"enrollmentStartDate\",\n        \"enrollmentEndDate\"\n      ]\n    },\n    \"eligibleLoyaltyTiers\": {\n    \
  \  \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tierGroup\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"name\",\n              \"id\"\n            ]\n          },\n          \"tier\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"\
  required\": [\n              \"name\",\n              \"id\"\n            ]\n          }\n        },\n        \"required\": [\n          \"tierGroup\",\n          \"tier\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"eligibleProductCategories\",\n    \"eligibleProducts\",\n    \"eligibleChannels\",\n    \"eligibleCustomerEvents\",\n    \"eligibleEnrollmentPeriod\",\n    \"eligibleLoyaltyTiers\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PromotionEligibility\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-promotion-eligibility-schema.json
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
title: PromotionEligibility
---
