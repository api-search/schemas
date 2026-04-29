---
description: CreateRefundRequest schema from Amazon Pay API
layout: schema
name: CreateRefundRequest
properties_list:
- description: ''
  name: chargeId
  type: string
- description: ''
  name: refundAmount
  type: object
- description: ''
  name: softDescriptor
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-create-refund-request-schema.json
slug: pay-create-refund-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"chargeId\",\n    \"refundAmount\"\n  ],\n  \"properties\": {\n    \"chargeId\": {\n      \"type\": \"string\"\n    },\n    \"refundAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"softDescriptor\": {\n      \"type\": \"string\",\n      \"maxLength\": 16\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateRefundRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-refund-request-schema.json\",\n  \"description\": \"CreateRefundRequest schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-refund-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateRefundRequest
---
