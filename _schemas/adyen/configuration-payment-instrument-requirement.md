---
description: PaymentInstrumentRequirement schema from Adyen API
layout: schema
name: PaymentInstrumentRequirement
properties_list:
- description: Specifies the requirements for the payment instrument that need to be included in the request for a particular route.
  name: description
  type: string
- description: The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the payment instrument is issued. For example, **NL** or **US**.
  name: issuingCountryCode
  type: string
- description: Specifies if the requirement only applies to transfers to another balance platform.
  name: onlyForCrossBalancePlatform
  type: boolean
- description: The type of the payment instrument. For example, "BankAccount" or "Card".
  name: paymentInstrumentType
  type: string
- description: '**paymentInstrumentRequirement**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-payment-instrument-requirement-schema.json
slug: configuration-payment-instrument-requirement
source_filename: configuration-payment-instrument-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-requirement-schema.json\",\n  \"title\": \"PaymentInstrumentRequirement\",\n  \"description\": \"PaymentInstrumentRequirement schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Specifies the requirements for the payment instrument that need to be included in the request for a particular route.\",\n      \"type\": \"string\"\n    },\n    \"issuingCountryCode\": {\n      \"description\": \"The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the payment instrument is issued. For example, **NL** or **US**.\",\n      \"type\": \"string\"\n    },\n    \"onlyForCrossBalancePlatform\": {\n      \"description\": \"Specifies if the requirement only applies to transfers\
  \ to another balance platform.\",\n      \"type\": \"boolean\"\n    },\n    \"paymentInstrumentType\": {\n      \"description\": \"The type of the payment instrument. For example, \\\"BankAccount\\\" or \\\"Card\\\".\",\n      \"enum\": [\n        \"BankAccount\",\n        \"Card\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"paymentInstrumentRequirement\",\n      \"description\": \"**paymentInstrumentRequirement**\",\n      \"enum\": [\n        \"paymentInstrumentRequirement\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-requirement-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentRequirement
---
