---
description: AT&T enterprise product order status and details
layout: schema
name: Product Order
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: externalId
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: orderDate
  type: string
- description: ''
  name: completionDate
  type:
  - string
  - 'null'
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/enterprise-apis-product-order-schema.json
slug: enterprise-apis-product-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://devex-web.att.com/schemas/enterprise/product-order\",\n  \"title\": \"Product Order\",\n  \"description\": \"AT&T enterprise product order status and details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"acknowledged\",\n        \"inProgress\",\n        \"pending\",\n        \"held\",\n        \"cancelled\",\n        \"completed\",\n        \"failed\",\n        \"partial\"\n      ]\n    },\n    \"orderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completionDate\": {\n      \"type\": [\n        \"string\",\n        \"null\"\n      ],\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/enterprise-apis-product-order-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Product Order
---
