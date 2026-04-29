---
description: Profile schema from Amazon Advertising API
layout: schema
name: Profile
properties_list:
- description: ''
  name: profileId
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: accountInfo
  type: object
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/advertising-profile-schema.json
slug: advertising-profile
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileId\": {\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"accountInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"marketplaceStringId\": {\n          \"type\": \"string\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"seller\",\n            \"vendor\"\n          ]\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Profile\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-profile-schema.json\",\n  \"description\": \"Profile schema from Amazon Advertising API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/advertising-profile-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Profile
---
