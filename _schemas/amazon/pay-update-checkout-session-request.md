---
description: UpdateCheckoutSessionRequest schema from Amazon Pay API
layout: schema
name: UpdateCheckoutSessionRequest
properties_list:
- description: ''
  name: paymentDetails
  type: object
- description: ''
  name: merchantMetadata
  type: object
- description: ''
  name: shippingAddress
  type: object
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-update-checkout-session-request-schema.json
slug: pay-update-checkout-session-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"paymentIntent\": {\n          \"type\": \"string\"\n        },\n        \"chargeAmount\": {\n          \"$ref\": \"#/components/schemas/Price\"\n        }\n      }\n    },\n    \"merchantMetadata\": {\n      \"$ref\": \"#/components/schemas/MerchantMetadata\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateCheckoutSessionRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-update-checkout-session-request-schema.json\",\n  \"description\": \"UpdateCheckoutSessionRequest schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-update-checkout-session-request-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: UpdateCheckoutSessionRequest
---
