---
description: FundRecipient schema from Adyen API
layout: schema
name: FundRecipient
properties_list:
- description: The address where to send the invoice.
  name: billingAddress
  type: object
- description: the used paymentMetohd
  name: paymentMethod
  type: object
- description: the email address of the person
  name: shopperEmail
  type: string
- description: the name of the person
  name: shopperName
  type: object
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: Required for Back-to-Back/ purchase driven load in Wallet transactions. Contains the final merchant who will be receiving the money, also known as subMerchant, information.
  name: subMerchant
  type: object
- description: the telephone number of the person
  name: telephoneNumber
  type: string
- description: indicates where the money is going
  name: walletIdentifier
  type: string
- description: indicates the tax identifier of the fund recepient
  name: walletOwnerTaxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-fund-recipient-schema.json
slug: checkout-fund-recipient
source_filename: checkout-fund-recipient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-fund-recipient-schema.json\",\n  \"title\": \"FundRecipient\",\n  \"description\": \"FundRecipient schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"paymentMethod\": {\n      \"description\": \"the used paymentMetohd\",\n      \"$ref\": \"#/components/schemas/CardDetails\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"the email address of the person\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"the name of the person\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference\
  \ to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"maxLength\": 256,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"subMerchant\": {\n      \"description\": \"Required for Back-to-Back/ purchase driven load in Wallet transactions.\\nContains the final merchant who will be receiving the money, also known as subMerchant, information.\",\n      \"$ref\": \"#/components/schemas/SubMerchant\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"the telephone number of the person\",\n      \"type\": \"string\"\n    },\n    \"walletIdentifier\": {\n      \"description\": \"indicates\
  \ where the money is going\",\n      \"type\": \"string\"\n    },\n    \"walletOwnerTaxId\": {\n      \"description\": \"indicates the tax identifier of the fund recepient\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-fund-recipient-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FundRecipient
---
