---
description: Tax address for a customer
layout: schema
name: Address
properties_list:
- description: Whether the address has been verified
  name: verified
  type: boolean
- description: Address line 1
  name: line1
  type: string
- description: State or province
  name: state
  type: string
- description: City
  name: city
  type: string
- description: Postal or ZIP code
  name: postalCode
  type: string
- description: ISO country code
  name: country
  type: string
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/billing-address-schema.json
slug: billing-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Tax address for a customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the address has been verified\"\n    },\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 1\",\n      \"example\": \"123 Main Street\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\",\n      \"example\": \"CA\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\",\n      \"example\": \"San Francisco\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\",\n      \"example\": \"94105\"\n    },\n    \"\
  country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO country code\",\n      \"example\": \"US\"\n    }\n  },\n  \"required\": [\n    \"line1\",\n    \"city\",\n    \"country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/billing-address-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: Address
---
