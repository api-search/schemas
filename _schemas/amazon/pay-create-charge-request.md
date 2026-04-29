---
description: CreateChargeRequest schema from Amazon Pay API
layout: schema
name: CreateChargeRequest
properties_list:
- description: ''
  name: chargePermissionId
  type: string
- description: ''
  name: chargeAmount
  type: object
- description: ''
  name: captureNow
  type: boolean
- description: ''
  name: softDescriptor
  type: string
- description: ''
  name: canHandlePendingAuthorization
  type: boolean
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-create-charge-request-schema.json
slug: pay-create-charge-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"chargePermissionId\",\n    \"chargeAmount\"\n  ],\n  \"properties\": {\n    \"chargePermissionId\": {\n      \"type\": \"string\"\n    },\n    \"chargeAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"captureNow\": {\n      \"type\": \"boolean\"\n    },\n    \"softDescriptor\": {\n      \"type\": \"string\",\n      \"maxLength\": 16\n    },\n    \"canHandlePendingAuthorization\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateChargeRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-charge-request-schema.json\",\n  \"description\": \"CreateChargeRequest schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-charge-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateChargeRequest
---
