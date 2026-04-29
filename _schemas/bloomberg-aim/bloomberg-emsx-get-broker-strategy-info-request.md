---
description: ''
layout: schema
name: GetBrokerStrategyInfoRequest
properties_list:
- description: ''
  name: EMSX_BROKER
  type: string
- description: ''
  name: EMSX_STRATEGY
  type: string
- description: ''
  name: EMSX_ASSET_CLASS
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-get-broker-strategy-info-request-schema.json
slug: bloomberg-emsx-get-broker-strategy-info-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetBrokerStrategyInfoRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_BROKER\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STRATEGY\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_ASSET_CLASS\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-get-broker-strategy-info-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GetBrokerStrategyInfoRequest
---
