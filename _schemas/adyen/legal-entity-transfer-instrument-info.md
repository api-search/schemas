---
description: TransferInstrumentInfo schema from Adyen API
layout: schema
name: TransferInstrumentInfo
properties_list:
- description: Contains information about the legal entity's bank account.
  name: bankAccount
  type: object
- description: The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) that owns the transfer instrument.
  name: legalEntityId
  type: string
- description: 'The type of transfer instrument. Possible value: **bankAccount**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-transfer-instrument-info-schema.json
slug: legal-entity-transfer-instrument-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-info-schema.json\",\n  \"title\": \"TransferInstrumentInfo\",\n  \"description\": \"TransferInstrumentInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccount\": {\n      \"description\": \"Contains information about the legal entity's bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccountInfo\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) that owns the transfer instrument.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of transfer instrument.\\n\\nPossible value: **bankAccount**.\",\n      \"enum\": [\n        \"bankAccount\",\n       \
  \ \"recurringDetail\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"legalEntityId\",\n    \"type\",\n    \"bankAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferInstrumentInfo
---
