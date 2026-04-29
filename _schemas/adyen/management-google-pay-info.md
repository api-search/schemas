---
description: GooglePayInfo schema from Adyen API
layout: schema
name: GooglePayInfo
properties_list:
- description: 'Google Pay [Merchant ID](https://support.google.com/paymentscenter/answer/7163092?hl=en). Character length and limitations: 16 alphanumeric characters or 20 numeric characters.'
  name: merchantId
  type: string
- description: 'Indicates whether the Google Pay Merchant ID is used for several merchant accounts. Default value: **false**.'
  name: reuseMerchantId
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-google-pay-info-schema.json
slug: management-google-pay-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-google-pay-info-schema.json\",\n  \"title\": \"GooglePayInfo\",\n  \"description\": \"GooglePayInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantId\": {\n      \"description\": \"Google Pay [Merchant ID](https://support.google.com/paymentscenter/answer/7163092?hl=en). Character length and limitations: 16 alphanumeric characters or 20 numeric characters.\",\n      \"maxLength\": 20,\n      \"minLength\": 16,\n      \"type\": \"string\"\n    },\n    \"reuseMerchantId\": {\n      \"description\": \"Indicates whether the Google Pay Merchant ID is used for several merchant accounts. Default value: **false**.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"merchantId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-google-pay-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GooglePayInfo
---
