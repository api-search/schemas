---
description: HistoricalRatesResponse schema from Abstract API exchange-rates
layout: schema
name: HistoricalRatesResponse
properties_list:
- description: Base currency code
  name: base
  type: string
- description: Historical date queried
  name: date
  type: string
- description: Map of currency codes to historical exchange rates
  name: exchange_rates
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/exchange-rates-historical-rates-response-schema.json
slug: exchange-rates-historical-rates-response
source_filename: exchange-rates-historical-rates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-historical-rates-response-schema.json\",\n  \"title\": \"HistoricalRatesResponse\",\n  \"description\": \"HistoricalRatesResponse schema from Abstract API exchange-rates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency code\",\n      \"example\": \"USD\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Historical date queried\",\n      \"example\": \"2026-01-01\"\n    },\n    \"exchange_rates\": {\n      \"type\": \"object\",\n      \"description\": \"Map of currency codes to historical exchange rates\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-historical-rates-response-schema.json
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
title: HistoricalRatesResponse
---
