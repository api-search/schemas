---
description: PaymentInstrumentGroup schema from Adyen API
layout: schema
name: PaymentInstrumentGroup
properties_list:
- description: The unique identifier of the [balance platform](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balancePlatforms/{id}__queryParam_id) to which the payment instrument group belongs.
  name: balancePlatform
  type: string
- description: Your description for the payment instrument group, maximum 300 characters.
  name: description
  type: string
- description: The unique identifier of the payment instrument group.
  name: id
  type: string
- description: Properties of the payment instrument group.
  name: properties
  type: object
- description: Your reference for the payment instrument group, maximum 150 characters.
  name: reference
  type: string
- description: The tx variant of the payment instrument group.
  name: txVariant
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-payment-instrument-group-schema.json
slug: configuration-payment-instrument-group
source_filename: configuration-payment-instrument-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-group-schema.json\",\n  \"title\": \"PaymentInstrumentGroup\",\n  \"description\": \"PaymentInstrumentGroup schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the [balance platform](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balancePlatforms/{id}__queryParam_id) to which the payment instrument group belongs.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the payment instrument group, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the payment instrument group.\",\n      \"type\": \"string\"\n\
  \    },\n    \"properties\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Properties of the payment instrument group.\",\n      \"type\": \"object\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment instrument group, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"txVariant\": {\n      \"description\": \"The tx variant of the payment instrument group.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"balancePlatform\",\n    \"txVariant\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-group-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentGroup
---
