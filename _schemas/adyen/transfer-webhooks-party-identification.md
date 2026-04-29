---
description: PartyIdentification schema from Adyen API
layout: schema
name: PartyIdentification
properties_list:
- description: Address of the bank account owner.
  name: address
  type: object
- description: The date of birth of the individual in [ISO-8601](https://www.w3.org/TR/NOTE-datetime) format. For example, **YYYY-MM-DD**. Should not be before January 1, 1900. Allowed only when `type` is **individu
  name: dateOfBirth
  type: string
- description: First name of the individual. Allowed only when `type` is **individual**.
  name: firstName
  type: string
- description: The name of the entity.
  name: fullName
  type: string
- description: Last name of the individual. Allowed only when `type` is **individual**.
  name: lastName
  type: string
- description: A unique reference to identify the party or counterparty involved in transfers. This identifier ensures consistency and uniqueness throughout all transactions initiated to and from the same party. For
  name: reference
  type: string
- description: 'The type of entity that owns the bank account. Possible values: **individual**, **organization**, or **unknown**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-party-identification-schema.json
slug: transfer-webhooks-party-identification
source_filename: transfer-webhooks-party-identification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-party-identification-schema.json\",\n  \"title\": \"PartyIdentification\",\n  \"description\": \"PartyIdentification schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"Address of the bank account owner.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"dateOfBirth\": {\n      \"description\": \"The date of birth of the individual in [ISO-8601](https://www.w3.org/TR/NOTE-datetime) format. For example, **YYYY-MM-DD**. Should not be before January 1, 1900.\\n\\nAllowed only when `type` is **individual**.\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"description\": \"First name of the individual.\\n\\nAllowed only when `type` is **individual**.\",\n      \"type\"\
  : \"string\"\n    },\n    \"fullName\": {\n      \"description\": \"The name of the entity.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"Last name of the individual.\\n\\nAllowed only when `type` is **individual**.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"A unique reference to identify the party or counterparty involved in transfers. This identifier ensures consistency and uniqueness throughout all transactions initiated to and from the same party. For example, your client's unique wallet or payee ID.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"unknown\",\n      \"description\": \"The type of entity that owns the bank account.\\n\\n Possible values: **individual**, **organization**, or **unknown**.\",\n      \"enum\": [\n        \"individual\",\n        \"organization\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n\
  \  \"required\": [\n    \"fullName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-party-identification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PartyIdentification
---
