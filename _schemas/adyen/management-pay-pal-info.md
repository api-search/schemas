---
description: PayPalInfo schema from Adyen API
layout: schema
name: PayPalInfo
properties_list:
- description: Indicates if direct (immediate) capture for PayPal is enabled. If set to **true**, this setting overrides the [capture](https://docs.adyen.com/online-payments/capture) settings of your merchant accoun
  name: directCapture
  type: boolean
- description: 'PayPal Merchant ID. Character length and limitations: 13 single-byte alphanumeric characters.'
  name: payerId
  type: string
- description: Your business email address.
  name: subject
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-pay-pal-info-schema.json
slug: management-pay-pal-info
source_filename: management-pay-pal-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pay-pal-info-schema.json\",\n  \"title\": \"PayPalInfo\",\n  \"description\": \"PayPalInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directCapture\": {\n      \"description\": \"Indicates if direct (immediate) capture for PayPal is enabled. If set to **true**, this setting overrides the [capture](https://docs.adyen.com/online-payments/capture) settings of your merchant account. Default value: **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"payerId\": {\n      \"description\": \"PayPal Merchant ID. Character length and limitations: 13 single-byte alphanumeric characters.\",\n      \"maxLength\": 13,\n      \"minLength\": 13,\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"description\": \"Your business email address.\",\n      \"type\": \"string\"\
  \n    }\n  },\n  \"required\": [\n    \"subject\",\n    \"payerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-pay-pal-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayPalInfo
---
