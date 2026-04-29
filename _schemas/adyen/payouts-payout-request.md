---
description: PayoutRequest schema from Adyen API
layout: schema
name: PayoutRequest
properties_list:
- description: The amount information for the transaction (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/
  name: amount
  type: object
- description: The address where to send the invoice. > The `billingAddress` object is required in the following scenarios. Include all of the fields within this object. >* For 3D Secure 2 transactions in all browse
  name: billingAddress
  type: object
- description: A container for card data. > Either `bankAccount` or `card` field must be provided in a payment request.
  name: card
  type: object
- description: An integer value that is added to the normal fraud score. The value can be either positive or negative.
  name: fraudOffset
  type: integer
- description: The person or entity funding the money.
  name: fundSource
  type: object
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The recurring settings for the payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/classic-integration/recurring-payments).
  name: recurring
  type: object
- description: The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a require
  name: reference
  type: string
- description: The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored recurring detail.
  name: selectedRecurringDetailReference
  type: string
- description: The shopper's email address. We recommend that you provide this data, as it is used in velocity fraud checks. > For 3D Secure 2 transactions, schemes require `shopperEmail` for all browser-based and m
  name: shopperEmail
  type: string
- description: Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer. For the web service API, Adyen assumes Ecommerce shopper interaction b
  name: shopperInteraction
  type: string
- description: The shopper's full name.
  name: shopperName
  type: object
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
- description: The shopper's telephone number.
  name: telephoneNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-payout-request-schema.json
slug: payouts-payout-request
source_filename: payouts-payout-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-payout-request-schema.json\",\n  \"title\": \"PayoutRequest\",\n  \"description\": \"PayoutRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount information for the transaction (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) requests, set amount to 0 (zero).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"billingAddress\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The address where to send the invoice.\\n> The `billingAddress` object is required in the following scenarios. Include all of the fields within this object.\\n>* For 3D Secure 2 transactions\
  \ in all browser-based and mobile implementations.\\n>* For cross-border payouts to and from Canada.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"card\": {\n      \"description\": \"A container for card data.\\n> Either `bankAccount` or `card` field must be provided in a payment request.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"fraudOffset\": {\n      \"description\": \"An integer value that is added to the normal fraud score. The value can be either positive or negative.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"fundSource\": {\n      \"x-addedInVersion\": \"64\",\n      \"description\": \"The person or entity funding the money.\",\n      \"$ref\": \"#/components/schemas/FundSource\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"recurring\": {\n      \"description\"\
  : \"The recurring settings for the payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/classic-integration/recurring-payments).\",\n      \"$ref\": \"#/components/schemas/Recurring\"\n    },\n    \"reference\": {\n      \"description\": \"The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a requirement.\\nIf you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\").\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"selectedRecurringDetailReference\": {\n      \"description\": \"The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address.\
  \ We recommend that you provide this data, as it is used in velocity fraud checks.\\n> For 3D Secure 2 transactions, schemes require `shopperEmail` for all browser-based and mobile implementations.\",\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer.\\nFor the web service API, Adyen assumes Ecommerce shopper interaction by default.\\n\\nThis field has the following possible values:\\n* `Ecommerce` - Online transactions where the cardholder is present (online). For better authorisation rates, we recommend sending the card security code (CSC) along with the request.\\n* `ContAuth` - Card on file and/or subscription transactions, where the cardholder is known to the merchant (returning customer). If the shopper is present (online), you can supply also the CSC to improve authorisation (one-click payment).\\n* `Moto` - Mail-order\
  \ and telephone-order transactions where the shopper is in contact with the merchant via email or telephone.\\n* `POS` - Point-of-sale transactions where the shopper is physically present to make a payment using a secure payment terminal.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The shopper's full name.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\"\
  : \"The shopper's telephone number.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-payout-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutRequest
---
