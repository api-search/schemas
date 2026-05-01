---
description: A virtual bank account issued through Decentro for collections or escrow.
layout: schema
name: Decentro Virtual Account
properties_list:
- description: ''
  name: account_number
  type: string
- description: ''
  name: ifsc
  type: string
- description: ''
  name: customer_id
  type: string
- description: ''
  name: purpose
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: balance
  type: number
- description: ''
  name: status
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Decentro
provider_slug: decentro
schema_file: json-schema/decentro-virtual-account.json
slug: decentro-virtual-account
source_filename: decentro-virtual-account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/decentro/json-schema/decentro-virtual-account.json\",\n  \"title\": \"Decentro Virtual Account\",\n  \"description\": \"A virtual bank account issued through Decentro for collections or escrow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_number\": {\"type\": \"string\"},\n    \"ifsc\": {\"type\": \"string\"},\n    \"customer_id\": {\"type\": \"string\"},\n    \"purpose\": {\"type\": \"string\"},\n    \"currency\": {\"type\": \"string\"},\n    \"balance\": {\"type\": \"number\"},\n    \"status\": {\"type\": \"string\", \"enum\": [\"ACTIVE\", \"FROZEN\", \"CLOSED\"]},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"}\n  },\n  \"required\": [\"account_number\", \"ifsc\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/decentro/refs/heads/main/json-schema/decentro-virtual-account.json
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
title: Decentro Virtual Account
---
