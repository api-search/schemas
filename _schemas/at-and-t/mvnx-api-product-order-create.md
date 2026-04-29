---
description: ProductOrderCreate schema from AT&T API
layout: schema
name: ProductOrderCreate
properties_list:
- description: External order identifier for tracking
  name: externalId
  type: string
- description: ''
  name: orderItem
  type: array
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-product-order-create-schema.json
slug: mvnx-api-product-order-create
source_filename: mvnx-api-product-order-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-order-create-schema.json\",\n  \"title\": \"ProductOrderCreate\",\n  \"description\": \"ProductOrderCreate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External order identifier for tracking\",\n      \"example\": \"ext-order-500123\"\n    },\n    \"orderItem\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"action\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"add\",\n              \"modify\",\n              \"delete\"\n            ],\n            \"example\": \"add\"\n          },\n          \"product\": {\n            \"type\": \"object\",\n            \"properties\": {\n         \
  \     \"productOffering\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"offer-unlimited-basic\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-order-create-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ProductOrderCreate
---
