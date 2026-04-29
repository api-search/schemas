---
description: ProductOrder schema from AT&T API
layout: schema
name: ProductOrder
properties_list:
- description: Unique product order identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Order state
  name: state
  type: string
- description: External order identifier
  name: externalId
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-product-order-schema.json
slug: mvnx-api-product-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-order-schema.json\",\n  \"title\": \"ProductOrder\",\n  \"description\": \"ProductOrder schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product order identifier\",\n      \"example\": \"order-500123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/productOrder/order-500123\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Order state\",\n      \"enum\": [\n        \"inProgress\",\n        \"completed\",\n        \"cancelled\",\n        \"failed\"\n      ],\n      \"example\": \"inProgress\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External\
  \ order identifier\",\n      \"example\": \"ext-order-500123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-order-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ProductOrder
---
