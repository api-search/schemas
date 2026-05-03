---
description: A credit limit managed through Traiana CreditLink, representing a real-time credit boundary for a counterparty relationship across asset classes.
layout: schema
name: Credit Limit
properties_list:
- description: Unique identifier for the credit limit
  name: limitId
  type: string
- description: Identifier of the counterparty
  name: counterpartyId
  type: string
- description: Name of the counterparty
  name: counterpartyName
  type: string
- description: Asset class the limit applies to
  name: assetClass
  type: string
- description: Type of trading relationship
  name: relationshipType
  type: string
- description: Maximum credit limit amount
  name: limitAmount
  type: number
- description: ISO 4217 currency code for the limit
  name: currency
  type: string
- description: Current utilization amount
  name: currentUtilization
  type: number
- description: Current utilization as a percentage of the limit
  name: utilizationPercentage
  type: number
- description: Current status of the credit limit
  name: status
  type: string
- description: Date the limit becomes effective
  name: effectiveDate
  type: string
- description: Date the limit expires
  name: expiryDate
  type: string
- description: Timestamp when the limit was created
  name: createdAt
  type: string
- description: Timestamp of the last update
  name: updatedAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/credit-limit.json
slug: credit-limit
source_filename: credit-limit.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/credit-limit.json\",\n  \"title\": \"Credit Limit\",\n  \"description\": \"A credit limit managed through Traiana CreditLink, representing a real-time credit boundary for a counterparty relationship across asset classes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limitId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the credit limit\"\n    },\n    \"counterpartyId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the counterparty\"\n    },\n    \"counterpartyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the counterparty\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class the limit applies to\",\n      \"enum\": [\"FX\", \"Equities\", \"EquityDerivatives\", \"ETD\"\
  , \"IRD\"]\n    },\n    \"relationshipType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of trading relationship\",\n      \"enum\": [\"PrimeBrokered\", \"Cleared\", \"Bilateral\"]\n    },\n    \"limitAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum credit limit amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the limit\"\n    },\n    \"currentUtilization\": {\n      \"type\": \"number\",\n      \"description\": \"Current utilization amount\"\n    },\n    \"utilizationPercentage\": {\n      \"type\": \"number\",\n      \"description\": \"Current utilization as a percentage of the limit\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the credit limit\",\n      \"enum\": [\"Active\", \"Suspended\", \"Terminated\"]\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\"\
  : \"Date the limit becomes effective\"\n    },\n    \"expiryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the limit expires\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the limit was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last update\"\n    }\n  },\n  \"required\": [\"limitId\", \"counterpartyId\", \"assetClass\", \"relationshipType\", \"limitAmount\", \"currency\", \"status\", \"effectiveDate\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/credit-limit.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Credit Limit
---
