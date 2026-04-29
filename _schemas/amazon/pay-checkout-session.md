---
description: CheckoutSession schema from Amazon Pay API
layout: schema
name: CheckoutSession
properties_list:
- description: ''
  name: checkoutSessionId
  type: string
- description: ''
  name: statusDetails
  type: object
- description: ''
  name: buyer
  type: object
- description: ''
  name: shippingAddress
  type: object
- description: ''
  name: billingAddress
  type: object
- description: ''
  name: paymentDetails
  type: object
- description: ''
  name: merchantMetadata
  type: object
- description: ''
  name: chargePermissionId
  type: string
- description: ''
  name: chargeId
  type: string
- description: ''
  name: creationTimestamp
  type: string
- description: ''
  name: expirationTimestamp
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-checkout-session-schema.json
slug: pay-checkout-session
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutSessionId\": {\n      \"type\": \"string\"\n    },\n    \"statusDetails\": {\n      \"$ref\": \"#/components/schemas/StatusDetails\"\n    },\n    \"buyer\": {\n      \"$ref\": \"#/components/schemas/Buyer\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"paymentDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"paymentIntent\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Confirm\",\n            \"Authorize\",\n            \"AuthorizeWithCapture\"\n          ]\n        },\n        \"chargeAmount\": {\n          \"$ref\": \"#/components/schemas/Price\"\n        }\n      }\n    },\n    \"merchantMetadata\": {\n      \"$ref\": \"#/components/schemas/MerchantMetadata\"\n    },\n    \"chargePermissionId\": {\n      \"type\": \"\
  string\"\n    },\n    \"chargeId\": {\n      \"type\": \"string\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"expirationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CheckoutSession\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-checkout-session-schema.json\",\n  \"description\": \"CheckoutSession schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-checkout-session-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: CheckoutSession
---
