---
description: TopupBalance schema from AT&T API
layout: schema
name: TopupBalance
properties_list:
- description: Unique top-up transaction identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Transaction status
  name: status
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-topup-balance-schema.json
slug: mvnx-api-topup-balance
source_filename: mvnx-api-topup-balance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-topup-balance-schema.json\",\n  \"title\": \"TopupBalance\",\n  \"description\": \"TopupBalance schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique top-up transaction identifier\",\n      \"example\": \"topup-500123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/topupBalance/topup-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction status\",\n      \"enum\": [\n        \"completed\",\n        \"failed\",\n        \"inProgress\"\n      ],\n      \"example\": \"completed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-topup-balance-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TopupBalance
---
