---
description: CostEstimateRequest schema from Adyen API
layout: schema
name: CostEstimateRequest
properties_list:
- description: The transaction amount used as a base for the cost estimation.
  name: amount
  type: object
- description: Assumptions made for the expected characteristics of the transaction, for which the charges are being estimated.
  name: assumptions
  type: object
- description: The card number (4-19 characters) for PCI compliant use cases. Do not use any separators. > Either the `cardNumber` or `encryptedCardNumber` field must be provided in a payment request.
  name: cardNumber
  type: string
- description: Encrypted data that stores card information for non PCI-compliant use cases. The encrypted data must be created with the Checkout Card Component or Secured Fields Component, and must contain the `encr
  name: encryptedCardNumber
  type: string
- description: The merchant account identifier you want to process the (transaction) request with.
  name: merchantAccount
  type: string
- description: Additional data for merchants who don't use Adyen as the payment authorisation gateway.
  name: merchantDetails
  type: object
- description: The recurring settings for the payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/online-payments/tokenization).
  name: recurring
  type: object
- description: The `recurringDetailReference` you want to use for this cost estimate. The value `LATEST` can be used to select the most recently stored recurring detail.
  name: selectedRecurringDetailReference
  type: string
- description: Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer. For the web service API, Adyen assumes Ecommerce shopper interaction b
  name: shopperInteraction
  type: string
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-cost-estimate-request-schema.json
slug: binlookup-cost-estimate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-request-schema.json\",\n  \"title\": \"CostEstimateRequest\",\n  \"description\": \"CostEstimateRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The transaction amount used as a base for the cost estimation.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"assumptions\": {\n      \"description\": \"Assumptions made for the expected characteristics of the transaction, for which the charges are being estimated.\",\n      \"$ref\": \"#/components/schemas/CostEstimateAssumptions\"\n    },\n    \"cardNumber\": {\n      \"description\": \"The card number (4-19 characters) for PCI compliant use cases. Do not use any separators.\\n\\n> Either the `cardNumber` or `encryptedCardNumber` field must be provided\
  \ in a payment request.\",\n      \"maxLength\": 19,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"encryptedCardNumber\": {\n      \"description\": \"Encrypted data that stores card information for non PCI-compliant use cases. The encrypted data must be created with the Checkout Card Component or Secured Fields Component, and must contain the `encryptedCardNumber` field.\\n\\n> Either the `cardNumber` or `encryptedCardNumber` field must be provided in a payment request.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier you want to process the (transaction) request with.\",\n      \"type\": \"string\"\n    },\n    \"merchantDetails\": {\n      \"description\": \"Additional data for merchants who don't use Adyen as the payment authorisation gateway.\",\n      \"$ref\": \"#/components/schemas/MerchantDetails\"\n    },\n    \"recurring\": {\n      \"description\": \"The recurring settings for the\
  \ payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/online-payments/tokenization).\",\n      \"$ref\": \"#/components/schemas/Recurring\"\n    },\n    \"selectedRecurringDetailReference\": {\n      \"description\": \"The `recurringDetailReference` you want to use for this cost estimate. The value `LATEST` can be used to select the most recently stored recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer.\\nFor the web service API, Adyen assumes Ecommerce shopper interaction by default.\\n\\nThis field has the following possible values:\\n* `Ecommerce` - Online transactions where the cardholder is present (online). For better authorisation rates, we recommend sending the card security code (CSC) along with the request.\\n* `ContAuth` - Card on file and/or\
  \ subscription transactions, where the card holder is known to the merchant (returning customer). If the shopper is present (online), you can supply also the CSC to improve authorisation (one-click payment).\\n* `Moto` - Mail-order and telephone-order transactions where the shopper is in contact with the merchant via email or telephone.\\n* `POS` - Point-of-sale transactions where the shopper is physically present to make a payment using a secure payment terminal.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\"\
  : [\n    \"amount\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CostEstimateRequest
---
