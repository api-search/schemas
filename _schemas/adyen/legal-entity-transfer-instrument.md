---
description: TransferInstrument schema from Adyen API
layout: schema
name: TransferInstrument
properties_list:
- description: Contains information about the legal entity's bank account.
  name: bankAccount
  type: object
- description: List of capabilities for this transfer instrument.
  name: capabilities
  type: object
- description: List of documents uploaded for the transfer instrument.
  name: documentDetails
  type: array
- description: The unique identifier of the transfer instrument.
  name: id
  type: string
- description: The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) that owns the transfer instrument.
  name: legalEntityId
  type: string
- description: The verification errors related to capabilities for this transfer instrument.
  name: problems
  type: array
- description: 'The type of transfer instrument. Possible value: **bankAccount**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-transfer-instrument-schema.json
slug: legal-entity-transfer-instrument
source_filename: legal-entity-transfer-instrument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-schema.json\",\n  \"title\": \"TransferInstrument\",\n  \"description\": \"TransferInstrument schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccount\": {\n      \"description\": \"Contains information about the legal entity's bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccountInfo\"\n    },\n    \"capabilities\": {\n      \"x-addedInVersion\": \"3\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/SupportingEntityCapability\"\n      },\n      \"description\": \"List of capabilities for this transfer instrument.\",\n      \"type\": \"object\"\n    },\n    \"documentDetails\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"List of documents uploaded for the transfer instrument.\",\n  \
  \    \"items\": {\n        \"$ref\": \"#/components/schemas/DocumentReference\"\n      },\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the transfer instrument.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/legalentity/latest/post/legalEntities#responses-200-id) that owns the transfer instrument.\",\n      \"type\": \"string\"\n    },\n    \"problems\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The verification errors related to capabilities for this transfer instrument.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CapabilityProblem\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"The type of transfer instrument.\\n\\nPossible value: **bankAccount**.\",\n      \"enum\": [\n        \"bankAccount\",\n \
  \       \"recurringDetail\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"legalEntityId\",\n    \"type\",\n    \"bankAccount\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-transfer-instrument-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferInstrument
---
