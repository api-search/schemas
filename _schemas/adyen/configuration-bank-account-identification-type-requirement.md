---
description: BankAccountIdentificationTypeRequirement schema from Adyen API
layout: schema
name: BankAccountIdentificationTypeRequirement
properties_list:
- description: 'List of bank account identification types: eg.; [iban , numberAndBic]'
  name: bankAccountIdentificationTypes
  type: array
- description: Specifies the bank account details for a particular route per required field in this object depending on the country of the bank account and the currency of the transfer.
  name: description
  type: string
- description: '**bankAccountIdentificationTypeRequirement**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-bank-account-identification-type-requirement-schema.json
slug: configuration-bank-account-identification-type-requirement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-identification-type-requirement-schema.json\",\n  \"title\": \"BankAccountIdentificationTypeRequirement\",\n  \"description\": \"BankAccountIdentificationTypeRequirement schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountIdentificationTypes\": {\n      \"description\": \"List of bank account identification types: eg.; [iban , numberAndBic]\",\n      \"items\": {\n        \"enum\": [\n          \"auLocal\",\n          \"brLocal\",\n          \"caLocal\",\n          \"czLocal\",\n          \"dkLocal\",\n          \"hkLocal\",\n          \"huLocal\",\n          \"iban\",\n          \"legacy\",\n          \"noLocal\",\n          \"numberAndBic\",\n          \"nzLocal\",\n          \"plLocal\",\n          \"seLocal\",\n          \"sgLocal\",\n         \
  \ \"ukLocal\",\n          \"usLocal\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"Specifies the bank account details for a particular route per required field in this object depending on the country of the bank account and the currency of the transfer.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"bankAccountIdentificationTypeRequirement\",\n      \"description\": \"**bankAccountIdentificationTypeRequirement**\",\n      \"enum\": [\n        \"bankAccountIdentificationTypeRequirement\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-identification-type-requirement-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountIdentificationTypeRequirement
---
