---
description: AdditionalDataSubMerchant schema from Adyen API
layout: schema
name: AdditionalDataSubMerchant
properties_list:
- description: Required for transactions performed by registered payment facilitators. Indicates the number of sub-merchants contained in the request. For example, **3**.
  name: subMerchant.numberOfSubSellers
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The city of the sub-merchant''s address. * Format: Alphanumeric * Maximum length: 13 characters'
  name: subMerchant.subSeller[subSellerNr].city
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The three-letter country code of the sub-merchant''s address. For example, **BRA** for Brazil. * Format: [ISO 3166-1 alpha-3](htt'
  name: subMerchant.subSeller[subSellerNr].country
  type: string
- description: 'Required for transactions performed by registered payment facilitators. A unique identifier that you create for the sub-merchant, used by schemes to identify the sub-merchant. * Format: Alphanumeric *'
  name: subMerchant.subSeller[subSellerNr].id
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The sub-merchant''s 4-digit Merchant Category Code (MCC). * Format: Numeric * Fixed length: 4 digits'
  name: subMerchant.subSeller[subSellerNr].mcc
  type: string
- description: Required for transactions performed by registered payment facilitators. The name of the sub-merchant. Based on scheme specifications, this value will overwrite the shopper statement that will appear i
  name: subMerchant.subSeller[subSellerNr].name
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The postal code of the sub-merchant''s address, without dashes. * Format: Numeric * Fixed length: 8 digits'
  name: subMerchant.subSeller[subSellerNr].postalCode
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The state code of the sub-merchant''s address, if applicable to the country. * Format: Alphanumeric * Maximum length: 2 character'
  name: subMerchant.subSeller[subSellerNr].state
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The street name and house number of the sub-merchant''s address. * Format: Alphanumeric * Maximum length: 60 characters'
  name: subMerchant.subSeller[subSellerNr].street
  type: string
- description: 'Required for transactions performed by registered payment facilitators. The tax ID of the sub-merchant. * Format: Numeric * Fixed length: 11 digits for the CPF or 14 digits for the CNPJ'
  name: subMerchant.subSeller[subSellerNr].taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-sub-merchant-schema.json
slug: checkout-additional-data-sub-merchant
source_filename: checkout-additional-data-sub-merchant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-sub-merchant-schema.json\",\n  \"title\": \"AdditionalDataSubMerchant\",\n  \"description\": \"AdditionalDataSubMerchant schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subMerchant.numberOfSubSellers\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. Indicates the number of sub-merchants contained in the request. For example, **3**.\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].city\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The city of the sub-merchant's address.\\n* Format: Alphanumeric\\n* Maximum length: 13 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].country\": {\n\
  \      \"description\": \"Required for transactions performed by registered payment facilitators. The three-letter country code of the sub-merchant's address. For example, **BRA** for Brazil. \\n* Format: [ISO 3166-1 alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3)\\n* Fixed length: 3 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].id\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. A unique identifier that you create for the sub-merchant, used by schemes to identify the sub-merchant. \\n* Format: Alphanumeric\\n* Maximum length: 15 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].mcc\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The sub-merchant's 4-digit Merchant Category Code (MCC). \\n* Format: Numeric\\n* Fixed length: 4 digits\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].name\"\
  : {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The name of the sub-merchant. Based on scheme specifications, this value will overwrite the shopper statement  that will appear in the card statement.\\n* Format: Alphanumeric\\n* Maximum length: 22 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].postalCode\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The postal code of the sub-merchant's address, without dashes.\\n* Format: Numeric\\n* Fixed length: 8 digits\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].state\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The state code of the sub-merchant's address, if applicable to the country.\\n* Format: Alphanumeric\\n* Maximum length: 2 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].street\"\
  : {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The street name and house number of the sub-merchant's address.\\n* Format: Alphanumeric\\n* Maximum length: 60 characters\",\n      \"type\": \"string\"\n    },\n    \"subMerchant.subSeller[subSellerNr].taxId\": {\n      \"description\": \"Required for transactions performed by registered payment facilitators. The tax ID of the sub-merchant.\\n* Format: Numeric\\n* Fixed length: 11 digits for the CPF or 14 digits for the CNPJ\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-sub-merchant-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataSubMerchant
---
