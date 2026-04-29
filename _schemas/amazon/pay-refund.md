---
description: Refund schema from Amazon Pay API
layout: schema
name: Refund
properties_list:
- description: ''
  name: refundId
  type: string
- description: ''
  name: chargeId
  type: string
- description: ''
  name: refundAmount
  type: object
- description: ''
  name: softDescriptor
  type: string
- description: ''
  name: statusDetails
  type: object
- description: ''
  name: creationTimestamp
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-refund-schema.json
slug: pay-refund
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"refundId\": {\n      \"type\": \"string\"\n    },\n    \"chargeId\": {\n      \"type\": \"string\"\n    },\n    \"refundAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"softDescriptor\": {\n      \"type\": \"string\"\n    },\n    \"statusDetails\": {\n      \"$ref\": \"#/components/schemas/StatusDetails\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Refund\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-refund-schema.json\",\n  \"description\": \"Refund schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-refund-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Refund
---
