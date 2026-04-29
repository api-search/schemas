---
description: A domestic payment initiation request for the Barclays Payment Initiation API.
layout: schema
name: PaymentRequest
properties_list:
- description: Unique identifier for the payment instruction assigned by the PISP.
  name: instructionIdentification
  type: string
- description: End-to-end reference for the payment.
  name: endToEndIdentification
  type: string
- description: ''
  name: instructedAmount
  type: object
- description: ''
  name: creditorAccount
  type: object
- description: ''
  name: remittanceInformation
  type: object
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/payment-schema.json
slug: payment
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/barclays/json-schema/payment-schema.json\",\n  \"title\": \"PaymentRequest\",\n  \"description\": \"A domestic payment initiation request for the Barclays Payment Initiation API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instructionIdentification\": {\n      \"type\": \"string\",\n      \"maxLength\": 35,\n      \"description\": \"Unique identifier for the payment instruction assigned by the PISP.\"\n    },\n    \"endToEndIdentification\": {\n      \"type\": \"string\",\n      \"maxLength\": 35,\n      \"description\": \"End-to-end reference for the payment.\"\n    },\n    \"instructedAmount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\"\
  \n        }\n      },\n      \"required\": [\"amount\", \"currency\"]\n    },\n    \"creditorAccount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"schemeName\": {\n          \"type\": \"string\",\n          \"enum\": [\"UK.OBIE.SortCodeAccountNumber\", \"UK.OBIE.IBAN\"]\n        },\n        \"identification\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"schemeName\", \"identification\", \"name\"]\n    },\n    \"remittanceInformation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": {\n          \"type\": \"string\",\n          \"maxLength\": 35\n        },\n        \"unstructured\": {\n          \"type\": \"string\",\n          \"maxLength\": 140\n        }\n      }\n    }\n  },\n  \"required\": [\"instructionIdentification\", \"endToEndIdentification\", \"instructedAmount\", \"creditorAccount\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/barclays/refs/heads/main/json-schema/payment-schema.json
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: PaymentRequest
---
