---
description: TransferInstrumentReference schema from Adyen API
layout: schema
name: TransferInstrumentReference
properties_list:
- description: The masked IBAN or bank account number.
  name: accountIdentifier
  type: string
- description: The unique identifier of the resource.
  name: id
  type: string
- description: Four last digits of the bank account number. If the transfer instrument is created using [instant bank account verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#relea
  name: realLastFour
  type: string
- description: Identifies if the bank account was created through [instant bank verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#releaseNote=2023-05-08-hosted-onboarding).
  name: trustedSource
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-transfer-instrument-reference-schema.json
slug: legal-entity-transfer-instrument-reference
source_filename: legal-entity-transfer-instrument-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-reference-schema.json\",\n  \"title\": \"TransferInstrumentReference\",\n  \"description\": \"TransferInstrumentReference schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIdentifier\": {\n      \"description\": \"The masked IBAN or bank account number.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"realLastFour\": {\n      \"description\": \"Four last digits of the bank account number. If the transfer instrument is created using [instant bank account verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#releaseNote=2023-05-08-hosted-onboarding), and it is a virtual bank account, these digits may be\
  \ different from the last four digits of the masked account number.\",\n      \"type\": \"string\"\n    },\n    \"trustedSource\": {\n      \"description\": \"Identifies if the bank account was created through [instant bank verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#releaseNote=2023-05-08-hosted-onboarding).\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"accountIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferInstrumentReference
---
