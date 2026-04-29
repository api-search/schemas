---
description: TopupBalanceCreate schema from AT&T API
layout: schema
name: TopupBalanceCreate
properties_list:
- description: ''
  name: channel
  type: object
- description: ''
  name: product
  type: object
- description: ''
  name: amount
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-topup-balance-create-schema.json
slug: mvnx-api-topup-balance-create
source_filename: mvnx-api-topup-balance-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-topup-balance-create-schema.json\",\n  \"title\": \"TopupBalanceCreate\",\n  \"description\": \"TopupBalanceCreate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"API\"\n        }\n      }\n    },\n    \"product\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Subscriber product ID\",\n          \"example\": \"sub-a1b2c3d4\"\n        }\n      }\n    },\n    \"amount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"units\": {\n          \"type\": \"number\",\n          \"description\": \"Top-up amount\",\n          \"\
  example\": 10.0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"Currency code (ISO 4217)\",\n          \"example\": \"USD\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-topup-balance-create-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TopupBalanceCreate
---
