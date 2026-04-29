---
description: PayoutMethod schema from Adyen API
layout: schema
name: PayoutMethod
properties_list:
- description: The [`merchantAccount`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_merchantAccount) you used in the `/payments` request when you [saved the account holder's c
  name: merchantAccount
  type: string
- description: Adyen-generated unique alphanumeric identifier (UUID) for the payout method, returned in the response when you create a payout method. Required when updating an existing payout method in an `/updateAc
  name: payoutMethodCode
  type: string
- description: Your reference for the payout method.
  name: payoutMethodReference
  type: string
- description: The [`recurringDetailReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_additionalData-ResponseAdditionalDataCommon-recurring-recurringDetailReference) re
  name: recurringDetailReference
  type: string
- description: The [`shopperReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_shopperReference) you sent in the `/payments` request when you [saved the account holder's
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-payout-method-schema.json
slug: notifications-payout-method
source_filename: notifications-payout-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-payout-method-schema.json\",\n  \"title\": \"PayoutMethod\",\n  \"description\": \"PayoutMethod schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The [`merchantAccount`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_merchantAccount) you used in the `/payments` request when you [saved the account holder's card details](https://docs.adyen.com/marketplaces-and-platforms/classic/payouts/manual-payout/payout-to-cards#check-and-store).\",\n      \"type\": \"string\"\n    },\n    \"payoutMethodCode\": {\n      \"description\": \"Adyen-generated unique alphanumeric identifier (UUID) for the payout method, returned in the response when you create a payout method. Required when updating an existing\
  \ payout method in an `/updateAccountHolder` request.\",\n      \"type\": \"string\"\n    },\n    \"payoutMethodReference\": {\n      \"description\": \"Your reference for the payout method.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The [`recurringDetailReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_additionalData-ResponseAdditionalDataCommon-recurring-recurringDetailReference)  returned in the `/payments` response when you [saved the account holder's card details](https://docs.adyen.com/marketplaces-and-platforms/classic/payouts/manual-payout/payout-to-cards#check-and-store).\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The [`shopperReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__reqParam_shopperReference) you sent in the `/payments` request when you [saved the account holder's card details](https://docs.adyen.com/marketplaces-and-platforms/classic/payouts/manual-payout/payout-to-cards#check-and-store).\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperReference\",\n    \"recurringDetailReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-payout-method-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutMethod
---
