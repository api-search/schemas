---
description: StoreCreationWithMerchantCodeRequest schema from Adyen API
layout: schema
name: StoreCreationWithMerchantCodeRequest
properties_list:
- description: The address of the store.
  name: address
  type: object
- description: The unique identifiers of the [business lines](https://docs.adyen.com/api-explorer/legalentity/latest/post/businessLines#responses-200-id) that the store is associated with. If not specified, the busi
  name: businessLineIds
  type: array
- description: Your description of the store.
  name: description
  type: string
- description: The unique identifier of the store, used by certain payment methods and tax authorities. Accepts up to 14 digits. Required for CNPJ in Brazil, in the format 00.000.000/00git00-00 separated by dots, sl
  name: externalReferenceId
  type: string
- description: The unique identifier of the merchant account that the store belongs to.
  name: merchantId
  type: string
- description: The phone number of the store, including '+' and country code in the [E.164](https://en.wikipedia.org/wiki/E.164) format. If passed in a different format, we convert and validate the phone number agai
  name: phoneNumber
  type: string
- description: 'Your reference to recognize the store by. Also known as the store code. Allowed characters: lowercase and uppercase letters without diacritics, numbers 0 through 9, hyphen (-), and underscore (_). If '
  name: reference
  type: string
- description: 'The store name to be shown on the shopper''s bank or credit card statement and on the shopper receipt. Maximum length: 22 characters; can''t be all numbers.'
  name: shopperStatement
  type: string
- description: Rules for Adyen for Platforms merchants to split the transaction amount and fees.
  name: splitConfiguration
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-store-creation-with-merchant-code-request-schema.json
slug: management-store-creation-with-merchant-code-request
source_filename: management-store-creation-with-merchant-code-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-store-creation-with-merchant-code-request-schema.json\",\n  \"title\": \"StoreCreationWithMerchantCodeRequest\",\n  \"description\": \"StoreCreationWithMerchantCodeRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the store.\",\n      \"$ref\": \"#/components/schemas/StoreLocation\"\n    },\n    \"businessLineIds\": {\n      \"description\": \"The unique identifiers of the [business lines](https://docs.adyen.com/api-explorer/legalentity/latest/post/businessLines#responses-200-id) that the store is associated with.\\nIf not specified, the business line of the merchant account is used. Required when there are multiple business lines under the merchant account.\",\n      \"items\": {\n        \"type\": \"string\"\n\
  \      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"Your description of the store.\",\n      \"type\": \"string\"\n    },\n    \"externalReferenceId\": {\n      \"description\": \"The unique identifier of the store, used by certain payment methods and tax authorities. Accepts up to 14 digits.\\n\\nRequired for CNPJ in Brazil, in the format 00.000.000/00git00-00 separated by dots, slashes, hyphens, or without separators.\\n\\nOptional for Zip in Australia and SIRET in France, required except for nonprofit organizations and incorporated associations.\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The unique identifier of the merchant account that the store belongs to.\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the store, including '+' and country code in the [E.164](https://en.wikipedia.org/wiki/E.164) format. If passed in a different\
  \ format, we convert and validate the phone number against E.164. \",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference to recognize the store by. Also known as the store code.\\n Allowed characters: lowercase and uppercase letters without diacritics, numbers 0 through 9, hyphen (-), and underscore (_).\\n\\nIf you do not provide a reference in your POST request, it is populated with the Adyen-generated [id](https://docs.adyen.com/api-explorer/Management/latest/post/stores#responses-200-id).\",\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"description\": \"The store name to be shown on the shopper's bank or credit card statement and on the shopper receipt.\\nMaximum length: 22 characters; can't be all numbers.\",\n      \"type\": \"string\"\n    },\n    \"splitConfiguration\": {\n      \"description\": \"Rules for Adyen for Platforms merchants to split the transaction amount and fees.\",\n      \"$ref\": \"#/components/schemas/StoreSplitConfiguration\"\
  \n    }\n  },\n  \"required\": [\n    \"description\",\n    \"shopperStatement\",\n    \"phoneNumber\",\n    \"address\",\n    \"merchantId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-store-creation-with-merchant-code-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoreCreationWithMerchantCodeRequest
---
