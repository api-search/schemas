---
description: AdditionalDataLevel23 schema from Adyen API
layout: schema
name: AdditionalDataLevel23
properties_list:
- description: 'The customer code. * Encoding: ASCII * Max length: 25 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.customerReference
  type: string
- description: 'The three-letter [ISO 3166-1 alpha-3 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) for the destination address. * Encoding: ASCII * Fixed length: 3 characters'
  name: enhancedSchemeData.destinationCountryCode
  type: string
- description: 'The postal code of the destination address. * Encoding: ASCII * Max length: 10 characters * Must not start with a space'
  name: enhancedSchemeData.destinationPostalCode
  type: string
- description: 'Destination state or province code. * Encoding: ASCII * Max length: 3 characters * Must not start with a space'
  name: enhancedSchemeData.destinationStateProvinceCode
  type: string
- description: 'The duty amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. * Encoding: Numeric * Max length: 12 characters'
  name: enhancedSchemeData.dutyAmount
  type: string
- description: 'The shipping amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. * Encoding: Numeric *Max length: 12 characters'
  name: enhancedSchemeData.freightAmount
  type: string
- description: 'The [UNSPC commodity code](https://www.unspsc.org/) of the item. * Encoding: ASCII * Max length: 12 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.itemDetailLine[itemNr].commodityCode
  type: string
- description: 'A description of the item. * Encoding: ASCII * Max length: 26 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.itemDetailLine[itemNr].description
  type: string
- description: 'The discount amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. * Encoding: Numeric * Max length: 12 characters'
  name: enhancedSchemeData.itemDetailLine[itemNr].discountAmount
  type: string
- description: 'The product code. * Encoding: ASCII. * Max length: 12 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.itemDetailLine[itemNr].productCode
  type: string
- description: 'The number of items. Must be an integer greater than zero. * Encoding: Numeric * Max length: 12 characters * Must not start with a space or be all spaces'
  name: enhancedSchemeData.itemDetailLine[itemNr].quantity
  type: string
- description: 'The total amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. * Max length: 12 characters * Must not start with a space or be al'
  name: enhancedSchemeData.itemDetailLine[itemNr].totalAmount
  type: string
- description: 'The unit of measurement for an item. * Encoding: ASCII Max length: 3 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.itemDetailLine[itemNr].unitOfMeasure
  type: string
- description: 'The unit price in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. * Encoding: Numeric * Max length: 12 characters * Must not be all zer'
  name: enhancedSchemeData.itemDetailLine[itemNr].unitPrice
  type: string
- description: 'The order date. * Format: `ddMMyy` * Encoding: ASCII * Max length: 6 characters'
  name: enhancedSchemeData.orderDate
  type: string
- description: 'The postal code of the address the item is shipped from. * Encoding: ASCII * Max length: 10 characters * Must not start with a space or be all spaces * Must not be all zeros.'
  name: enhancedSchemeData.shipFromPostalCode
  type: string
- description: 'The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * For example, 2000 means USD 20.00. *Encoding: Numeric *Max length: 12 characters * Must not be al'
  name: enhancedSchemeData.totalTaxAmount
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-level23-schema.json
slug: checkout-additional-data-level23
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-level23-schema.json\",\n  \"title\": \"AdditionalDataLevel23\",\n  \"description\": \"AdditionalDataLevel23 schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enhancedSchemeData.customerReference\": {\n      \"description\": \"The customer code.\\n* Encoding: ASCII\\n* Max length: 25 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.destinationCountryCode\": {\n      \"description\": \"The three-letter [ISO 3166-1 alpha-3 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) for the destination address.\\n* Encoding: ASCII\\n* Fixed length: 3 characters\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.destinationPostalCode\": {\n     \
  \ \"description\": \"The postal code of the destination address.\\n* Encoding: ASCII\\n* Max length: 10 characters\\n* Must not start with a space\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.destinationStateProvinceCode\": {\n      \"description\": \"Destination state or province code.\\n* Encoding: ASCII\\n* Max length: 3 characters\\n* Must not start with a space\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.dutyAmount\": {\n      \"description\": \"The duty amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n* Encoding: Numeric\\n* Max length: 12 characters\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.freightAmount\": {\n      \"description\": \"The shipping amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n* Encoding: Numeric\\n*Max length: 12 characters\",\n      \"type\"\
  : \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].commodityCode\": {\n      \"description\": \"The [UNSPC commodity code](https://www.unspsc.org/) of the item.\\n* Encoding: ASCII\\n* Max length: 12 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].description\": {\n      \"description\": \"A description of the item.\\n* Encoding: ASCII\\n* Max length: 26 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].discountAmount\": {\n      \"description\": \"The discount amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n* Encoding: Numeric\\n* Max length: 12 characters\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].productCode\"\
  : {\n      \"description\": \"The product code.\\n* Encoding: ASCII.\\n* Max length: 12 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].quantity\": {\n      \"description\": \"The number of items. Must be an integer greater than zero.\\n* Encoding: Numeric\\n* Max length: 12 characters\\n* Must not start with a space or be all spaces\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].totalAmount\": {\n      \"description\": \"The total amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n* Max length: 12 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].unitOfMeasure\": {\n      \"description\": \"The unit of measurement for\
  \ an item.\\n* Encoding: ASCII\\n\\nMax length: 3 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.itemDetailLine[itemNr].unitPrice\": {\n      \"description\": \"The unit price in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n* Encoding: Numeric\\n* Max length: 12 characters\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.orderDate\": {\n      \"description\": \"The order date.\\n* Format: `ddMMyy`\\n* Encoding: ASCII\\n* Max length: 6 characters\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.shipFromPostalCode\": {\n      \"description\": \"The postal code of the address the item is shipped from.\\n* Encoding: ASCII\\n* Max length: 10 characters\\n* Must not start with a space or be all spaces\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n\
  \    },\n    \"enhancedSchemeData.totalTaxAmount\": {\n      \"description\": \"The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* For example, 2000 means USD 20.00.\\n*Encoding: Numeric\\n*Max length: 12 characters\\n* Must not be all zeros.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-level23-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataLevel23
---
