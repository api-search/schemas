---
description: ''
layout: schema
name: GetBrokerStrategiesRequest
properties_list:
- description: Broker code
  name: EMSX_BROKER
  type: string
- description: Asset class
  name: EMSX_ASSET_CLASS
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-get-broker-strategies-request-schema.json
slug: bloomberg-emsx-get-broker-strategies-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetBrokerStrategiesRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_BROKER\": {\n      \"type\": \"string\",\n      \"description\": \"Broker code\"\n    },\n    \"EMSX_ASSET_CLASS\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-get-broker-strategies-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GetBrokerStrategiesRequest
---
