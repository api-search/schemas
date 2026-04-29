---
description: FundDestination schema from Adyen API
layout: schema
name: FundDestination
properties_list:
- description: a map of name/value pairs for passing in additional/industry-specific data
  name: additionalData
  type: object
- description: The address where to send the invoice.
  name: billingAddress
  type: object
- description: Credit card data. Optional if `shopperReference` and `selectedRecurringDetailReference` are provided.
  name: card
  type: object
- description: The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored recurring detail.
  name: selectedRecurringDetailReference
  type: string
- description: the email address of the person
  name: shopperEmail
  type: string
- description: the name of the person
  name: shopperName
  type: object
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
- description: Required for Back-to-Back/ purchase driven load in Wallet transactions. Contains the final merchant who will be receiving the money, also known as subMerchant, information.
  name: subMerchant
  type: object
- description: the telephone number of the person
  name: telephoneNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-fund-destination-schema.json
slug: payments-fund-destination
source_filename: payments-fund-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fund-destination-schema.json\",\n  \"title\": \"FundDestination\",\n  \"description\": \"FundDestination schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"a map of name/value pairs for passing in additional/industry-specific data\",\n      \"type\": \"object\"\n    },\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"card\": {\n      \"description\": \"Credit card data.\\n\\nOptional if `shopperReference` and `selectedRecurringDetailReference` are provided.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"selectedRecurringDetailReference\"\
  : {\n      \"description\": \"The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"the email address of the person\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"the name of the person\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    },\n    \"subMerchant\": {\n      \"description\": \"Required for Back-to-Back/ purchase driven load in Wallet transactions.\\nContains the final merchant who will be receiving\
  \ the money, also known as subMerchant, information.\",\n      \"$ref\": \"#/components/schemas/SubMerchant\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"the telephone number of the person\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-fund-destination-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: FundDestination
---
