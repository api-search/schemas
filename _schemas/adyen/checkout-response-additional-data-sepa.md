---
description: ResponseAdditionalDataSepa schema from Adyen API
layout: schema
name: ResponseAdditionalDataSepa
properties_list:
- description: 'The transaction signature date. Format: yyyy-MM-dd'
  name: sepadirectdebit.dateOfSignature
  type: string
- description: Its value corresponds to the pspReference value of the transaction.
  name: sepadirectdebit.mandateId
  type: string
- description: 'This field can take one of the following values: * OneOff: (OOFF) Direct debit instruction to initiate exactly one direct debit transaction. * First: (FRST) Initial/first collection in a series of dir'
  name: sepadirectdebit.sequenceType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-response-additional-data-sepa-schema.json
slug: checkout-response-additional-data-sepa
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-additional-data-sepa-schema.json\",\n  \"title\": \"ResponseAdditionalDataSepa\",\n  \"description\": \"ResponseAdditionalDataSepa schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sepadirectdebit.dateOfSignature\": {\n      \"description\": \"The transaction signature date.\\n\\nFormat: yyyy-MM-dd\",\n      \"type\": \"string\"\n    },\n    \"sepadirectdebit.mandateId\": {\n      \"description\": \"Its value corresponds to the pspReference value of the transaction.\",\n      \"type\": \"string\"\n    },\n    \"sepadirectdebit.sequenceType\": {\n      \"description\": \"This field can take one of the following values:\\n* OneOff: (OOFF) Direct debit instruction to initiate exactly one direct debit transaction.\\n\\n* First: (FRST) Initial/first collection in a series\
  \ of direct debit instructions.\\n* Recurring: (RCUR) Direct debit instruction to carry out regular direct debit transactions initiated by the creditor.\\n* Final: (FNAL) Last/final collection in a series of direct debit instructions.\\n\\nExample: OOFF\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-additional-data-sepa-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataSepa
---
