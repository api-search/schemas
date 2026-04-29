---
description: IbanAccountIdentification schema from Adyen API
layout: schema
name: IbanAccountIdentification
properties_list:
- description: The international bank account number as defined in the [ISO-13616](https://www.iso.org/standard/81090.html) standard.
  name: iban
  type: string
- description: '**iban**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-iban-account-identification-schema.json
slug: configuration-iban-account-identification
source_filename: configuration-iban-account-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-iban-account-identification-schema.json\",\n  \"title\": \"IbanAccountIdentification\",\n  \"description\": \"IbanAccountIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iban\": {\n      \"description\": \"The international bank account number as defined in the [ISO-13616](https://www.iso.org/standard/81090.html) standard.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"iban\",\n      \"description\": \"**iban**\",\n      \"enum\": [\n        \"iban\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"iban\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-iban-account-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: IbanAccountIdentification
---
