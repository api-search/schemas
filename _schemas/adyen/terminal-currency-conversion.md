---
description: A currency conversion occurred in the payment, and the merchant needs to know information related to this conversion (e.g. to print on the sale receipt). Information related to a currency conversion.
layout: schema
name: CurrencyConversion
properties_list:
- description: Notify if the customer has approved something. Indicates if the customer has accepted a currency conversion.
  name: CustomerApprovedFlag
  type: boolean
- description: ''
  name: ConvertedAmount
  type: object
- description: Rate of currency conversion.
  name: Rate
  type: string
- description: Markup of a currency conversion amount as a percentage.
  name: Markup
  type: string
- description: Commission for a currency conversion.
  name: Commission
  type: number
- description: If a declaration has to be presented to the customer.
  name: Declaration
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-currency-conversion-schema.json
slug: terminal-currency-conversion
source_filename: terminal-currency-conversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-currency-conversion-schema.json\",\n  \"title\": \"CurrencyConversion\",\n  \"description\": \"A currency conversion occurred in the payment, and the merchant needs to know information related to this conversion (e.g. to print on the sale receipt). Information related to a currency conversion.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerApprovedFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Notify if the customer has approved something. Indicates if the customer has accepted a currency conversion.\"\n    },\n    \"ConvertedAmount\": {\n      \"$ref\": \"#/components/schemas/ConvertedAmount\"\n    },\n    \"Rate\": {\n      \"type\": \"string\",\n      \"description\": \"Rate of currency conversion.\"\n    },\n    \"Markup\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Markup of a currency conversion amount as a percentage.\"\n    },\n    \"Commission\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Commission for a currency conversion.\"\n    },\n    \"Declaration\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If a declaration has to be presented to the customer.\"\n    }\n  },\n  \"required\": [\n    \"ConvertedAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-currency-conversion-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CurrencyConversion
---
