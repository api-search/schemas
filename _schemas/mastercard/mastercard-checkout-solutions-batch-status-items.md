---
description: ''
layout: schema
name: BatchStatusItems
properties_list:
- description: 'The action to be performed on the Digital Payment Application (DPA). The selected action will be applied to all DPAs provided in the items list. __ADD__ - Add DPA __UPDATE__ - Update DPA __DELETE__ - '
  name: action
  type: string
- description: A unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded.
  name: serviceId
  type: string
- description: Token Requestors receive a unique identifier, TRID, which represents the consumer-facing entity name to the Issuer during the tokenization process. This identifier has a one-to-one relationship with t
  name: trid
  type: string
- description: 'The Cardholder facing name of the Merchant. Conditional: Must be supplied when adding Merchants to a Payment Facilitator (PF) program."'
  name: programName
  type: string
- description: Indicates the status of an individual Digital Payment Application (DPA) item in a batch.
  name: status
  type: string
- description: ''
  name: dpaResults
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-batch-status-items-schema.json
slug: mastercard-checkout-solutions-batch-status-items
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchStatusItems\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to be performed on the Digital Payment Application (DPA). The selected action will be applied to all DPAs provided in the items list.\\n\\n__ADD__ - Add DPA\\n\\n__UPDATE__ - Update DPA\\n\\n__DELETE__ - Delete DPA\\n\\nNote: A limited number of DPA fields can be changed using the 'UPDATE' action. These are dpaPresentationName, dpaLogoUri, debitTokenRequested,  merchantCategoryCode, and threeDSDefaultData. Please refer to the example for a minimal use case.\\n\"\n    },\n    \"serviceId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded.\"\n    },\n    \"trid\": {\n      \"type\": \"string\",\n      \"description\": \"Token Requestors\
  \ receive a unique identifier, TRID, which represents the consumer-facing entity name to the Issuer\\nduring the tokenization process. This identifier has a one-to-one relationship with the serviceId.\\n<br>\\n<br> Note: Reach out to your Mastercard representative to begin receiving trid in API responses.\\n\"\n    },\n    \"programName\": {\n      \"type\": \"string\",\n      \"description\": \"The Cardholder facing name of the Merchant.\\n\\nConditional: Must be supplied when adding Merchants to a Payment Facilitator (PF) program.\\\"\\n\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the status of an individual Digital Payment Application (DPA) item in a batch.\"\n    },\n    \"dpaResults\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-batch-status-items-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BatchStatusItems
---
