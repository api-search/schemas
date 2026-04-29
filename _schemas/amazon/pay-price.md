---
description: Price schema from Amazon Pay API
layout: schema
name: Price
properties_list:
- description: ''
  name: amount
  type: string
- description: ''
  name: currencyCode
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-price-schema.json
slug: pay-price
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"amount\",\n    \"currencyCode\"\n  ],\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Price\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-price-schema.json\",\n  \"description\": \"Price schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-price-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Price
---
