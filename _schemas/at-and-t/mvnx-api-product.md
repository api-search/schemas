---
description: Product schema from AT&T API
layout: schema
name: Product
properties_list:
- description: Unique product/subscriber identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Product status
  name: status
  type: string
- description: ''
  name: productOffering
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-product-schema.json
slug: mvnx-api-product
source_filename: mvnx-api-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"Product schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product/subscriber identifier\",\n      \"example\": \"sub-a1b2c3d4\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/product/sub-a1b2c3d4\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Product status\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"terminated\"\n      ],\n      \"example\": \"active\"\n    },\n    \"productOffering\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"\
  string\",\n          \"example\": \"offer-unlimited-basic\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Unlimited Basic Plan\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-product-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: Product
---
