---
description: Country definition with regulatory details
layout: schema
name: Country
properties_list:
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: Full country name
  name: countryName
  type: string
- description: Default currency code
  name: currencyCode
  type: string
- description: Whether IBAN is required for payments to this country
  name: ibanRequired
  type: boolean
- description: Whether the country is under sanctions
  name: sanctioned
  type: boolean
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-country-schema.json
slug: temenos-transact-core-banking-country
source_filename: temenos-transact-core-banking-country-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Country\",\n  \"type\": \"object\",\n  \"description\": \"Country definition with regulatory details\",\n  \"properties\": {\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"countryName\": {\n      \"type\": \"string\",\n      \"description\": \"Full country name\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Default currency code\"\n    },\n    \"ibanRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether IBAN is required for payments to this country\"\n    },\n    \"sanctioned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the country is under sanctions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-country-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Country
---
