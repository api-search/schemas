---
description: ResponseAdditionalDataBillingAddress schema from Adyen API
layout: schema
name: ResponseAdditionalDataBillingAddress
properties_list:
- description: The billing address city passed in the payment request.
  name: billingAddress.city
  type: string
- description: 'The billing address country passed in the payment request. Example: NL'
  name: billingAddress.country
  type: string
- description: The billing address house number or name passed in the payment request.
  name: billingAddress.houseNumberOrName
  type: string
- description: 'The billing address postal code passed in the payment request. Example: 1011 DJ'
  name: billingAddress.postalCode
  type: string
- description: 'The billing address state or province passed in the payment request. Example: NH'
  name: billingAddress.stateOrProvince
  type: string
- description: The billing address street passed in the payment request.
  name: billingAddress.street
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-response-additional-data-billing-address-schema.json
slug: payouts-response-additional-data-billing-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data-billing-address-schema.json\",\n  \"title\": \"ResponseAdditionalDataBillingAddress\",\n  \"description\": \"ResponseAdditionalDataBillingAddress schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddress.city\": {\n      \"description\": \"The billing address city passed in the payment request.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.country\": {\n      \"description\": \"The billing address country passed in the payment request.\\n\\nExample: NL\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.houseNumberOrName\": {\n      \"description\": \"The billing address house number or name passed in the payment request.\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.postalCode\": {\n      \"description\":\
  \ \"The billing address postal code passed in the payment request.\\n\\nExample: 1011 DJ\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.stateOrProvince\": {\n      \"description\": \"The billing address state or province passed in the payment request.\\n\\nExample: NH\",\n      \"type\": \"string\"\n    },\n    \"billingAddress.street\": {\n      \"description\": \"The billing address street passed in the payment request.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data-billing-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataBillingAddress
---
