---
description: ConvertResponse schema from Abstract API exchange-rates
layout: schema
name: ConvertResponse
properties_list:
- description: Source currency code
  name: base_currency
  type: string
- description: Target currency code
  name: target_currency
  type: string
- description: Original amount
  name: base_amount
  type: number
- description: Converted amount
  name: converted_amount
  type: number
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/exchange-rates-convert-response-schema.json
slug: exchange-rates-convert-response
source_filename: exchange-rates-convert-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-convert-response-schema.json\",\n  \"title\": \"ConvertResponse\",\n  \"description\": \"ConvertResponse schema from Abstract API exchange-rates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Source currency code\",\n      \"example\": \"USD\"\n    },\n    \"target_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Target currency code\",\n      \"example\": \"EUR\"\n    },\n    \"base_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Original amount\",\n      \"example\": 100\n    },\n    \"converted_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Converted amount\",\n      \"example\": 92.34\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-convert-response-schema.json
tags:
- Avatars
- Company Enrichment
- Contacts
- Currencies
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
title: ConvertResponse
---
