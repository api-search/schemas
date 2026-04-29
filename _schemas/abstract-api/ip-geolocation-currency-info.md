---
description: CurrencyInfo schema from Abstract API ip-geolocation
layout: schema
name: CurrencyInfo
properties_list:
- description: Currency full name
  name: currency_name
  type: string
- description: ISO 4217 currency code
  name: currency_code
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-geolocation-currency-info-schema.json
slug: ip-geolocation-currency-info
source_filename: ip-geolocation-currency-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-currency-info-schema.json\",\n  \"title\": \"CurrencyInfo\",\n  \"description\": \"CurrencyInfo schema from Abstract API ip-geolocation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency_name\": {\n      \"type\": \"string\",\n      \"description\": \"Currency full name\",\n      \"example\": \"US Dollar\"\n    },\n    \"currency_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-geolocation-currency-info-schema.json
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
title: CurrencyInfo
---
