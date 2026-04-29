---
description: IBAN validation and enrichment response
layout: schema
name: IBANValidationResponse
properties_list:
- description: The IBAN submitted for validation
  name: iban
  type: string
- description: Whether the IBAN is valid
  name: is_valid
  type: boolean
- description: ''
  name: country
  type: object
- description: ''
  name: bank
  type: object
- description: Account number extracted from the IBAN
  name: account_number
  type: string
- description: Check digits from the IBAN
  name: check_digits
  type: string
- description: Whether the country is a SEPA member
  name: sepa_member
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/iban-validation-iban-validation-response-schema.json
slug: iban-validation-iban-validation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/iban-validation-iban-validation-response-schema.json\",\n  \"title\": \"IBANValidationResponse\",\n  \"description\": \"IBAN validation and enrichment response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iban\": {\n      \"type\": \"string\",\n      \"description\": \"The IBAN submitted for validation\",\n      \"example\": \"GB82WEST12345698765432\"\n    },\n    \"is_valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the IBAN is valid\",\n      \"example\": true\n    },\n    \"country\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\",\n          \"example\": \"GB\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Country name\",\n          \"example\": \"United Kingdom\"\n        }\n      }\n    },\n    \"bank\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"bank_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the bank\",\n          \"example\": \"Westpac Banking Corporation\"\n        },\n        \"bank_code\": {\n          \"type\": \"string\",\n          \"description\": \"Bank identifier code within the IBAN\",\n          \"example\": \"WEST\"\n        },\n        \"bic\": {\n          \"type\": \"string\",\n          \"description\": \"Bank Identifier Code (BIC/SWIFT)\",\n          \"example\": \"WESTGB22\"\n        }\n      }\n    },\n    \"account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Account number extracted from the IBAN\",\n      \"example\": \"98765432\"\n    },\n    \"check_digits\": {\n      \"type\": \"string\",\n      \"description\": \"Check digits from the IBAN\",\n      \"example\"\
  : \"82\"\n    },\n    \"sepa_member\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the country is a SEPA member\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/iban-validation-iban-validation-response-schema.json
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
title: IBANValidationResponse
---
