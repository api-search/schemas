---
description: StoredValueIssueRequest schema from Adyen API
layout: schema
name: StoredValueIssueRequest
properties_list:
- description: The amount information for the transaction.
  name: amount
  type: object
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The collection that contains the type of the payment method and its specific information if available
  name: paymentMethod
  type: object
- description: ''
  name: recurringDetailReference
  type: string
- description: The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a require
  name: reference
  type: string
- description: Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer. For the web service API, Adyen assumes Ecommerce shopper interaction b
  name: shopperInteraction
  type: string
- description: ''
  name: shopperReference
  type: string
- description: The physical store, for which this payment is processed.
  name: store
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/stored-value-stored-value-issue-request-schema.json
slug: stored-value-stored-value-issue-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-issue-request-schema.json\",\n  \"title\": \"StoredValueIssueRequest\",\n  \"description\": \"StoredValueIssueRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount information for the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethod\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The collection that contains the type of the payment method and its specific information if available\",\n      \"type\": \"object\"\n    },\n    \"recurringDetailReference\"\
  : {\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a requirement.\\nIf you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\").\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer.\\nFor the web service API, Adyen assumes Ecommerce shopper interaction by default.\\n\\nThis field has the following possible values:\\n* `Ecommerce` - Online transactions where the cardholder is present (online). For better authorisation rates, we recommend sending the card security code (CSC) along with the request.\\n* `ContAuth` - Card on\
  \ file and/or subscription transactions, where the cardholder is known to the merchant (returning customer). If the shopper is present (online), you can supply also the CSC to improve authorisation (one-click payment).\\n* `Moto` - Mail-order and telephone-order transactions where the shopper is in contact with the merchant via email or telephone.\\n* `POS` - Point-of-sale transactions where the shopper is physically present to make a payment using a secure payment terminal.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"The physical store, for which this payment is processed.\",\n      \"maxLength\": 16,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\",\n    \"paymentMethod\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/stored-value-stored-value-issue-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredValueIssueRequest
---
