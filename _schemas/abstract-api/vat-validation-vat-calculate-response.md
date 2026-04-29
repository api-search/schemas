---
description: VATCalculateResponse schema from Abstract API vat-validation
layout: schema
name: VATCalculateResponse
properties_list:
- description: Amount excluding VAT
  name: amount_excl_vat
  type: number
- description: VAT amount
  name: vat_amount
  type: number
- description: Amount including VAT
  name: amount_incl_vat
  type: number
- description: VAT category used
  name: vat_category
  type: string
- description: VAT rate applied
  name: vat_rate
  type: number
- description: ''
  name: country_code
  type: string
- description: ''
  name: country_name
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/vat-validation-vat-calculate-response-schema.json
slug: vat-validation-vat-calculate-response
source_filename: vat-validation-vat-calculate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-calculate-response-schema.json\",\n  \"title\": \"VATCalculateResponse\",\n  \"description\": \"VATCalculateResponse schema from Abstract API vat-validation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount_excl_vat\": {\n      \"type\": \"number\",\n      \"description\": \"Amount excluding VAT\",\n      \"example\": 100\n    },\n    \"vat_amount\": {\n      \"type\": \"number\",\n      \"description\": \"VAT amount\",\n      \"example\": 19\n    },\n    \"amount_incl_vat\": {\n      \"type\": \"number\",\n      \"description\": \"Amount including VAT\",\n      \"example\": 119\n    },\n    \"vat_category\": {\n      \"type\": \"string\",\n      \"description\": \"VAT category used\",\n      \"example\": \"standard\"\n    },\n    \"vat_rate\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"VAT rate applied\",\n      \"example\": 19\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"example\": \"DE\"\n    },\n    \"country_name\": {\n      \"type\": \"string\",\n      \"example\": \"Germany\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-calculate-response-schema.json
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
title: VATCalculateResponse
---
