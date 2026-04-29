---
description: VATRatesResponse schema from Abstract API vat-validation
layout: schema
name: VATRatesResponse
properties_list:
- description: ''
  name: country_code
  type: string
- description: ''
  name: country_name
  type: string
- description: Standard VAT rate percentage
  name: standard_rate
  type: number
- description: Reduced VAT rate percentages
  name: reduced_rates
  type: array
- description: Super reduced VAT rate if applicable
  name: super_reduced_rate
  type: number
- description: Parking VAT rate if applicable
  name: parking_rate
  type: number
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/vat-validation-vat-rates-response-schema.json
slug: vat-validation-vat-rates-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-rates-response-schema.json\",\n  \"title\": \"VATRatesResponse\",\n  \"description\": \"VATRatesResponse schema from Abstract API vat-validation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country_code\": {\n      \"type\": \"string\",\n      \"example\": \"DE\"\n    },\n    \"country_name\": {\n      \"type\": \"string\",\n      \"example\": \"Germany\"\n    },\n    \"standard_rate\": {\n      \"type\": \"number\",\n      \"description\": \"Standard VAT rate percentage\",\n      \"example\": 19\n    },\n    \"reduced_rates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Reduced VAT rate percentages\",\n      \"example\": [\n        7\n      ]\n    },\n    \"super_reduced_rate\": {\n      \"type\": \"number\"\
  ,\n      \"nullable\": true,\n      \"description\": \"Super reduced VAT rate if applicable\",\n      \"example\": null\n    },\n    \"parking_rate\": {\n      \"type\": \"number\",\n      \"nullable\": true,\n      \"description\": \"Parking VAT rate if applicable\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-rates-response-schema.json
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
title: VATRatesResponse
---
