---
description: VATValidationResponse schema from Abstract API vat-validation
layout: schema
name: VATValidationResponse
properties_list:
- description: The VAT number validated
  name: vat_number
  type: string
- description: Whether the VAT number is valid
  name: valid
  type: boolean
- description: ''
  name: company
  type: object
- description: ''
  name: country
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/vat-validation-vat-validation-response-schema.json
slug: vat-validation-vat-validation-response
source_filename: vat-validation-vat-validation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-validation-response-schema.json\",\n  \"title\": \"VATValidationResponse\",\n  \"description\": \"VATValidationResponse schema from Abstract API vat-validation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vat_number\": {\n      \"type\": \"string\",\n      \"description\": \"The VAT number validated\",\n      \"example\": \"GB123456789\"\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the VAT number is valid\",\n      \"example\": true\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Company name associated with the VAT number\",\n          \"example\": \"Example Ltd\"\n        },\n        \"address\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Company address\",\n          \"example\": \"1 Example Street, London, UK\"\n        }\n      }\n    },\n    \"country\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Country code\",\n          \"example\": \"GB\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Country name\",\n          \"example\": \"United Kingdom\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/vat-validation-vat-validation-response-schema.json
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
title: VATValidationResponse
---
