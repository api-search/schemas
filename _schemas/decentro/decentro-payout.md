---
description: A disbursement initiated via Decentro's Payments API.
layout: schema
name: Decentro Payout
properties_list:
- description: ''
  name: transfer_id
  type: string
- description: ''
  name: from_account
  type: string
- description: ''
  name: to_account
  type: string
- description: ''
  name: to_ifsc
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: purpose_message
  type: string
- description: ''
  name: transfer_type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Decentro
provider_slug: decentro
schema_file: json-schema/decentro-payout.json
slug: decentro-payout
source_filename: decentro-payout.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/decentro/json-schema/decentro-payout.json\",\n  \"title\": \"Decentro Payout\",\n  \"description\": \"A disbursement initiated via Decentro's Payments API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transfer_id\": {\"type\": \"string\"},\n    \"from_account\": {\"type\": \"string\"},\n    \"to_account\": {\"type\": \"string\"},\n    \"to_ifsc\": {\"type\": \"string\"},\n    \"amount\": {\"type\": \"number\"},\n    \"currency\": {\"type\": \"string\"},\n    \"purpose_message\": {\"type\": \"string\"},\n    \"transfer_type\": {\"type\": \"string\", \"enum\": [\"IMPS\", \"NEFT\", \"RTGS\", \"UPI\"]},\n    \"status\": {\"type\": \"string\"},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"}\n  },\n  \"required\": [\"transfer_id\", \"amount\", \"transfer_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/json-schema/decentro-payout.json
tags:
- Banking
- Banking-as-a-Service
- FinTech
- India
- KYC
- Ledger
- Payments
- UPI
- Virtual Accounts
title: Decentro Payout
---
