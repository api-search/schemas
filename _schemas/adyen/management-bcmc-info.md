---
description: BcmcInfo schema from Adyen API
layout: schema
name: BcmcInfo
properties_list:
- description: Indicates if [Bancontact mobile](https://docs.adyen.com/payment-methods/bancontact/bancontact-mobile) is enabled.
  name: enableBcmcMobile
  type: boolean
- description: Information regarding the transaction description.
  name: transactionDescription
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-bcmc-info-schema.json
slug: management-bcmc-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-bcmc-info-schema.json\",\n  \"title\": \"BcmcInfo\",\n  \"description\": \"BcmcInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enableBcmcMobile\": {\n      \"description\": \"Indicates if [Bancontact mobile](https://docs.adyen.com/payment-methods/bancontact/bancontact-mobile) is enabled.\",\n      \"type\": \"boolean\"\n    },\n    \"transactionDescription\": {\n      \"description\": \"Information regarding the transaction description.\",\n      \"$ref\": \"#/components/schemas/TransactionDescriptionInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-bcmc-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BcmcInfo
---
