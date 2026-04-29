---
description: PhoneCountry schema from Abstract API phone-intelligence
layout: schema
name: PhoneCountry
properties_list:
- description: ISO 3166-1 alpha-2 country code
  name: code
  type: string
- description: Country name
  name: name
  type: string
- description: International dialing prefix
  name: prefix
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/phone-intelligence-phone-country-schema.json
slug: phone-intelligence-phone-country
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/phone-intelligence-phone-country-schema.json\",\n  \"title\": \"PhoneCountry\",\n  \"description\": \"PhoneCountry schema from Abstract API phone-intelligence\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\",\n      \"example\": \"US\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Country name\",\n      \"example\": \"United States\"\n    },\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"International dialing prefix\",\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/phone-intelligence-phone-country-schema.json
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
title: PhoneCountry
---
