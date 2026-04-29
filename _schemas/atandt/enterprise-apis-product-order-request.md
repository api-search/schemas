---
description: Request to create an AT&T enterprise service order
layout: schema
name: Product Order Request
properties_list:
- description: ''
  name: externalId
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: requestedStartDate
  type: string
- description: ''
  name: orderItem
  type: array
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/enterprise-apis-product-order-request-schema.json
slug: enterprise-apis-product-order-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://devex-web.att.com/schemas/enterprise/product-order-request\",\n  \"title\": \"Product Order Request\",\n  \"description\": \"Request to create an AT&T enterprise service order\",\n  \"type\": \"object\",\n  \"required\": [\n    \"orderItem\"\n  ],\n  \"properties\": {\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"requestedStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"orderItem\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"action\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"add\",\n              \"modify\",\n              \"delete\",\n              \"noChange\"\n            ]\n         \
  \ },\n          \"productOffering\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/enterprise-apis-product-order-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Product Order Request
---
