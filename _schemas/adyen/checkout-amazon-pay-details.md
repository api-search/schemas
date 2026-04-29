---
description: AmazonPayDetails schema from Adyen API
layout: schema
name: AmazonPayDetails
properties_list:
- description: This is the `amazonPayToken` that you obtained from the [Get Checkout Session](https://amazon-pay-acquirer-guide.s3-eu-west-1.amazonaws.com/v1/amazon-pay-api-v2/checkout-session.html#get-checkout-sess
  name: amazonPayToken
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The `checkoutSessionId` is used to identify the checkout session at the Amazon Pay side. This field is required only for drop-in and components integration, where it replaces the amazonPayToken.
  name: checkoutSessionId
  type: string
- description: '**amazonpay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-amazon-pay-details-schema.json
slug: checkout-amazon-pay-details
source_filename: checkout-amazon-pay-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-amazon-pay-details-schema.json\",\n  \"title\": \"AmazonPayDetails\",\n  \"description\": \"AmazonPayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amazonPayToken\": {\n      \"description\": \"This is the `amazonPayToken` that you obtained from the [Get Checkout Session](https://amazon-pay-acquirer-guide.s3-eu-west-1.amazonaws.com/v1/amazon-pay-api-v2/checkout-session.html#get-checkout-session) response. This token is used for API only integration specifically.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"checkoutSessionId\": {\n      \"description\": \"The `checkoutSessionId` is used to identify the\
  \ checkout session at the Amazon Pay side. This field is required only for drop-in and components integration, where it replaces the amazonPayToken.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"amazonpay\",\n      \"description\": \"**amazonpay**\",\n      \"enum\": [\n        \"amazonpay\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-amazon-pay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AmazonPayDetails
---
