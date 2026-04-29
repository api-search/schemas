---
description: CreateCheckoutSessionRequest schema from Amazon Pay API
layout: schema
name: CreateCheckoutSessionRequest
properties_list:
- description: ''
  name: webCheckoutDetails
  type: object
- description: ''
  name: storeId
  type: string
- description: ''
  name: chargePermissionType
  type: string
- description: ''
  name: paymentDetails
  type: object
- description: ''
  name: merchantMetadata
  type: object
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-create-checkout-session-request-schema.json
slug: pay-create-checkout-session-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"webCheckoutDetails\",\n    \"storeId\"\n  ],\n  \"properties\": {\n    \"webCheckoutDetails\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"checkoutReviewReturnUrl\"\n      ],\n      \"properties\": {\n        \"checkoutReviewReturnUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"checkoutResultReturnUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"storeId\": {\n      \"type\": \"string\"\n    },\n    \"chargePermissionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OneTime\",\n        \"Recurring\"\n      ]\n    },\n    \"paymentDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"paymentIntent\": {\n          \"type\": \"string\"\n        },\n        \"chargeAmount\": {\n          \"$ref\": \"#/components/schemas/Price\"\n        }\n      }\n    },\n \
  \   \"merchantMetadata\": {\n      \"$ref\": \"#/components/schemas/MerchantMetadata\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCheckoutSessionRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-checkout-session-request-schema.json\",\n  \"description\": \"CreateCheckoutSessionRequest schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-create-checkout-session-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CreateCheckoutSessionRequest
---
