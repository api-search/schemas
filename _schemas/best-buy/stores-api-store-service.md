---
description: A service offered at a Best Buy store.
layout: schema
name: StoreService
properties_list:
- description: Name of the service offered.
  name: service
  type: string
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/stores-api-store-service-schema.json
slug: stores-api-store-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-service-schema.json\",\n  \"title\": \"StoreService\",\n  \"description\": \"A service offered at a Best Buy store.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service offered.\",\n      \"example\": \"Geek Squad\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/stores-api-store-service-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: StoreService
---
