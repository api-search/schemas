---
description: PhoneNumber from WhatsApp API
layout: schema
name: PhoneNumber
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: display_phone_number
  type: string
- description: ''
  name: verified_name
  type: string
- description: ''
  name: quality_rating
  type: string
- description: ''
  name: code_verification_status
  type: string
- description: ''
  name: is_official_business_account
  type: boolean
- description: ''
  name: name_status
  type: string
- description: ''
  name: platform_type
  type: string
- description: ''
  name: throughput
  type: object
- description: ''
  name: account_mode
  type: string
- description: ''
  name: messaging_limit_tier
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-phone-number-schema.json
slug: whatsapp-business-management-api-phone-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-phone-number-schema.json\",\n  \"title\": \"PhoneNumber\",\n  \"description\": \"PhoneNumber from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"display_phone_number\": {\n      \"type\": \"string\",\n      \"example\": \"+15551234567\"\n    },\n    \"verified_name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"quality_rating\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GREEN\",\n        \"YELLOW\",\n        \"RED\",\n        \"UNKNOWN\"\n      ],\n      \"example\": \"GREEN\"\n    },\n    \"code_verification_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"VERIFIED\",\n        \"NOT_VERIFIED\"\
  ,\n        \"EXPIRED\"\n      ],\n      \"example\": \"VERIFIED\"\n    },\n    \"is_official_business_account\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name_status\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"platform_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CLOUD_API\",\n        \"ON_PREMISE\",\n        \"NOT_APPLICABLE\"\n      ],\n      \"example\": \"CLOUD_API\"\n    },\n    \"throughput\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"STANDARD\",\n            \"HIGH\"\n          ]\n        }\n      }\n    },\n    \"account_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LIVE\",\n        \"SANDBOX\"\n      ],\n      \"example\": \"LIVE\"\n    },\n    \"messaging_limit_tier\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TIER_1K\",\n       \
  \ \"TIER_10K\",\n        \"TIER_100K\",\n        \"TIER_UNLIMITED\"\n      ],\n      \"example\": \"TIER_1K\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-phone-number-schema.json
tags: []
title: PhoneNumber
---
