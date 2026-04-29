---
description: ResponseAdditionalDataDomesticError schema from Adyen API
layout: schema
name: ResponseAdditionalDataDomesticError
properties_list:
- description: The reason the transaction was declined, given by the local issuer. Currently available for merchants in Japan.
  name: domesticRefusalReasonRaw
  type: string
- description: The action the shopper should take, in a local language. Currently available in Japanese, for merchants in Japan.
  name: domesticShopperAdvice
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-response-additional-data-domestic-error-schema.json
slug: payments-response-additional-data-domestic-error
source_filename: payments-response-additional-data-domestic-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-domestic-error-schema.json\",\n  \"title\": \"ResponseAdditionalDataDomesticError\",\n  \"description\": \"ResponseAdditionalDataDomesticError schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domesticRefusalReasonRaw\": {\n      \"description\": \"The reason the transaction was declined, given by the local issuer. \\nCurrently available for merchants in Japan.\",\n      \"type\": \"string\"\n    },\n    \"domesticShopperAdvice\": {\n      \"description\": \"The action the shopper should take, in a local language. \\nCurrently available in Japanese, for merchants in Japan.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-domestic-error-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataDomesticError
---
