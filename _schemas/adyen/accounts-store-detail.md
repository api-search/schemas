---
description: StoreDetail schema from Adyen API
layout: schema
name: StoreDetail
properties_list:
- description: The address of the physical store where the account holder will process payments from.
  name: address
  type: object
- description: 'The phone number of the store provided as a single string. It will be handled as a landline phone. Examples: "0031 6 11 22 33 44", "+316/1122-3344", "(0031) 611223344"'
  name: fullPhoneNumber
  type: string
- description: Store logo for payment method setup.
  name: logo
  type: string
- description: The merchant account to which the store belongs.
  name: merchantAccount
  type: string
- description: The merchant category code (MCC) that classifies the business of the account holder.
  name: merchantCategoryCode
  type: string
- description: Merchant house number for payment method setup.
  name: merchantHouseNumber
  type: string
- description: The phone number of the store.
  name: phoneNumber
  type: object
- description: 'The sales channel. Possible values: **Ecommerce**, **POS**.'
  name: shopperInteraction
  type: string
- description: The unique reference for the split configuration, returned when you configure splits in your Customer Area. When this is provided, the `virtualAccount` is also required. Adyen uses the configuration a
  name: splitConfigurationUUID
  type: string
- description: 'The status of the store. Possible values: **Pending**, **Active**, **Inactive**, **InactiveWithModifications**, **Closed**.'
  name: status
  type: string
- description: Adyen-generated unique alphanumeric identifier (UUID) for the store, returned in the response when you create a store. Required when updating an existing store in an `/updateAccountHolder` request.
  name: store
  type: string
- description: 'The name of the account holder''s store. This value is shown in shopper statements. * Length: Between 3 to 22 characters * The following characters are *not* supported: **:;}{$#@!|<>%^*+=\\**'
  name: storeName
  type: string
- description: 'Your unique identifier for the store. The Customer Area also uses this value for the store description. * Length: Between 3 to 128 characters * The following characters are *not* supported: **:;}{$#@!'
  name: storeReference
  type: string
- description: The account holder's `accountCode` where the split amount will be sent. Required when you provide the `splitConfigurationUUID`.
  name: virtualAccount
  type: string
- description: URL of the ecommerce store.
  name: webAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-store-detail-schema.json
slug: accounts-store-detail
source_filename: accounts-store-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-store-detail-schema.json\",\n  \"title\": \"StoreDetail\",\n  \"description\": \"StoreDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the physical store where the account holder will process payments from.\",\n      \"$ref\": \"#/components/schemas/ViasAddress\"\n    },\n    \"fullPhoneNumber\": {\n      \"description\": \"The phone number of the store provided as a single string.  It will be handled as a landline phone.\\n\\nExamples: \\\"0031 6 11 22 33 44\\\", \\\"+316/1122-3344\\\", \\\"(0031) 611223344\\\"\",\n      \"type\": \"string\"\n    },\n    \"logo\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Store logo for payment method setup.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\"\
  : {\n      \"description\": \"The merchant account to which the store belongs.\",\n      \"type\": \"string\"\n    },\n    \"merchantCategoryCode\": {\n      \"description\": \"The merchant category code (MCC) that classifies the business of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"merchantHouseNumber\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Merchant house number for payment method setup.\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the store.\",\n      \"$ref\": \"#/components/schemas/ViasPhoneNumber\"\n    },\n    \"shopperInteraction\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The sales channel. Possible values: **Ecommerce**, **POS**.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"splitConfigurationUUID\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The unique\
  \ reference for the split configuration, returned when you configure splits in your Customer Area. When this is provided, the `virtualAccount` is also required. Adyen uses the configuration and the `virtualAccount` to split funds between accounts in your platform.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the store. Possible values: **Pending**, **Active**, **Inactive**, **InactiveWithModifications**, **Closed**.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"InactiveWithModifications\",\n        \"Pending\"\n      ],\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"Adyen-generated unique alphanumeric identifier (UUID) for the store, returned in the response when you create a store. Required when updating an existing store in an `/updateAccountHolder` request.\",\n      \"type\": \"string\"\n    },\n    \"storeName\": {\n      \"description\": \"The\
  \ name of the account holder's store. This value is shown in shopper statements.\\n\\n* Length: Between 3 to 22 characters \\n\\n* The following characters are *not* supported: **:;}{$#@!|<>%^*+=\\\\\\\\**\",\n      \"type\": \"string\"\n    },\n    \"storeReference\": {\n      \"description\": \"Your unique identifier for the store. The Customer Area also uses this value for the store description.\\n\\n * Length: Between 3 to 128 characters\\n\\n* The following characters are *not* supported: **:;}{$#@!|<>%^*+=\\\\\\\\**\",\n      \"type\": \"string\"\n    },\n    \"virtualAccount\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The account holder's `accountCode` where the split amount will be sent. Required when you provide the `splitConfigurationUUID`.\",\n      \"type\": \"string\"\n    },\n    \"webAddress\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"URL of the ecommerce store.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n\
  \    \"merchantCategoryCode\",\n    \"address\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-store-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoreDetail
---
