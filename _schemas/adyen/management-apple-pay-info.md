---
description: ApplePayInfo schema from Adyen API
layout: schema
name: ApplePayInfo
properties_list:
- description: 'The list of merchant domains. Maximum: 99 domains per request. For more information, see [Apple Pay documentation](https://docs.adyen.com/payment-methods/apple-pay/web-drop-in?tab=adyen-certificate-li'
  name: domains
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-apple-pay-info-schema.json
slug: management-apple-pay-info
source_filename: management-apple-pay-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-apple-pay-info-schema.json\",\n  \"title\": \"ApplePayInfo\",\n  \"description\": \"ApplePayInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domains\": {\n      \"description\": \"The list of merchant domains. Maximum: 99 domains per request.\\n\\nFor more information, see [Apple Pay documentation](https://docs.adyen.com/payment-methods/apple-pay/web-drop-in?tab=adyen-certificate-live_1#going-live).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"domains\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-apple-pay-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApplePayInfo
---
