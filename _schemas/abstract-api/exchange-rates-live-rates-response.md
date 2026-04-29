---
description: LiveRatesResponse schema from Abstract API exchange-rates
layout: schema
name: LiveRatesResponse
properties_list:
- description: Base currency code
  name: base
  type: string
- description: Unix timestamp of last update
  name: last_updated
  type: integer
- description: Map of currency codes to exchange rates
  name: exchange_rates
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/exchange-rates-live-rates-response-schema.json
slug: exchange-rates-live-rates-response
source_filename: exchange-rates-live-rates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-live-rates-response-schema.json\",\n  \"title\": \"LiveRatesResponse\",\n  \"description\": \"LiveRatesResponse schema from Abstract API exchange-rates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency code\",\n      \"example\": \"USD\"\n    },\n    \"last_updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of last update\",\n      \"example\": 1713518400\n    },\n    \"exchange_rates\": {\n      \"type\": \"object\",\n      \"description\": \"Map of currency codes to exchange rates\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/exchange-rates-live-rates-response-schema.json
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
title: LiveRatesResponse
---
