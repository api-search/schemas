---
description: PartyIdentification-2 schema from Adyen API
layout: schema
name: PartyIdentification-2
properties_list:
- description: Address of the bank account owner.
  name: address
  type: object
- description: First name of the individual. Required when `type` is **individual**.
  name: firstName
  type: string
- description: The name of the entity.
  name: fullName
  type: string
- description: Last name of the individual. Required when `type` is **individual**.
  name: lastName
  type: string
- description: 'The type of entity that owns the bank account. Possible values: **individual**, **organization**, or **unknown**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-party-identification-2-schema.json
slug: accounting-notifications-party-identification-2
source_filename: accounting-notifications-party-identification-2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-party-identification-2-schema.json\",\n  \"title\": \"PartyIdentification-2\",\n  \"description\": \"PartyIdentification-2 schema from Adyen API\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"Address of the bank account owner.\",\n      \"$ref\": \"#/components/schemas/Address-2\"\n    },\n    \"firstName\": {\n      \"description\": \"First name of the individual. Required when `type` is **individual**.\",\n      \"type\": \"string\"\n    },\n    \"fullName\": {\n      \"description\": \"The name of the entity.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"Last name of the individual. Required when `type` is **individual**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"unknown\",\n      \"description\"\
  : \"The type of entity that owns the bank account.\\n\\n Possible values: **individual**, **organization**, or **unknown**.\",\n      \"enum\": [\n        \"individual\",\n        \"organization\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"fullName\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-party-identification-2-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PartyIdentification-2
---
