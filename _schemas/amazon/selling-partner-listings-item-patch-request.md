---
description: ListingsItemPatchRequest schema from Amazon Selling Partner API
layout: schema
name: ListingsItemPatchRequest
properties_list:
- description: ''
  name: productType
  type: string
- description: ''
  name: patches
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-listings-item-patch-request-schema.json
slug: selling-partner-listings-item-patch-request
source_filename: selling-partner-listings-item-patch-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"productType\",\n    \"patches\"\n  ],\n  \"properties\": {\n    \"productType\": {\n      \"type\": \"string\"\n    },\n    \"patches\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"op\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"add\",\n              \"replace\",\n              \"delete\"\n            ]\n          },\n          \"path\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListingsItemPatchRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-patch-request-schema.json\"\
  ,\n  \"description\": \"ListingsItemPatchRequest schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-patch-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ListingsItemPatchRequest
---
