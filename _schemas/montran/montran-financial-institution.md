---
description: A financial institution participating in payment processing through Montran's infrastructure. Used to identify banks, clearing members, and financial intermediaries in payment transactions, aligned with ISO 20022 financial institution identification structures.
layout: schema
name: Montran Financial Institution
properties_list:
- description: Bank Identifier Code (SWIFT/BIC) - ISO 9362
  name: bic
  type: string
- description: Full legal name of the financial institution
  name: name
  type: string
- description: Legal Entity Identifier (ISO 17442)
  name: lei
  type: string
- description: Clearing system member identification (e.g., ABA routing number, sort code)
  name: clearingSystemMemberId
  type: string
- description: Clearing system in which the institution is a member
  name: clearingSystem
  type: string
- description: Country of registration (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Postal address of the institution
  name: address
  type: object
- description: Clearing and settlement systems the institution connects to via Montran
  name: connectedClearingSystems
  type: array
- description: Message formats supported by the institution
  name: supportedMessageFormats
  type: array
provider_name: Montran
provider_slug: montran
schema_file: json-schema/montran-financial-institution-schema.json
slug: montran-financial-institution
source_filename: montran-financial-institution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.montran.com/schemas/financial-institution.json\",\n  \"title\": \"Montran Financial Institution\",\n  \"description\": \"A financial institution participating in payment processing through Montran's infrastructure. Used to identify banks, clearing members, and financial intermediaries in payment transactions, aligned with ISO 20022 financial institution identification structures.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"bic\"\n  ],\n  \"properties\": {\n    \"bic\": {\n      \"type\": \"string\",\n      \"description\": \"Bank Identifier Code (SWIFT/BIC) - ISO 9362\",\n      \"pattern\": \"^[A-Z]{4}[A-Z]{2}[A-Z0-9]{2}([A-Z0-9]{3})?$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full legal name of the financial institution\"\n    },\n    \"lei\": {\n      \"type\": \"string\",\n      \"description\": \"Legal Entity Identifier (ISO 17442)\"\
  ,\n      \"pattern\": \"^[A-Z0-9]{20}$\"\n    },\n    \"clearingSystemMemberId\": {\n      \"type\": \"string\",\n      \"description\": \"Clearing system member identification (e.g., ABA routing number, sort code)\"\n    },\n    \"clearingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Clearing system in which the institution is a member\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of registration (ISO 3166-1 alpha-2)\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"Postal address of the institution\",\n      \"properties\": {\n        \"streetName\": {\n          \"type\": \"string\"\n        },\n        \"buildingNumber\": {\n          \"type\": \"string\"\n        },\n        \"postCode\": {\n          \"type\": \"string\"\n        },\n        \"townName\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\"\
  : \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"connectedClearingSystems\": {\n      \"type\": \"array\",\n      \"description\": \"Clearing and settlement systems the institution connects to via Montran\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"SEPA\",\n          \"TARGET2\",\n          \"FEDWIRE\",\n          \"CHIPS\",\n          \"CHAPS\",\n          \"FASTER_PAYMENTS\",\n          \"TIPS\",\n          \"RT1\",\n          \"RTGS\",\n          \"ACH\",\n          \"SWIFT\"\n        ]\n      }\n    },\n    \"supportedMessageFormats\": {\n      \"type\": \"array\",\n      \"description\": \"Message formats supported by the institution\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"SWIFT_FIN\",\n          \"ISO20022\",\n          \"ISO8583\",\n          \"NACHA\",\n          \"PROPRIETARY\"\n        ]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/json-schema/montran-financial-institution-schema.json
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
title: Montran Financial Institution
---
