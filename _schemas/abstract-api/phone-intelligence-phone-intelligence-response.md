---
description: Phone number intelligence response
layout: schema
name: PhoneIntelligenceResponse
properties_list:
- description: The phone number in E.164 format
  name: phone
  type: string
- description: Whether the phone number is valid
  name: valid
  type: boolean
- description: ''
  name: country
  type: object
- description: Geographic location of the phone number
  name: location
  type: string
- description: Line type
  name: type
  type: string
- description: Carrier or service provider
  name: carrier
  type: string
- description: Whether the number is a VoIP number
  name: is_voip
  type: boolean
- description: Risk score from 0 (low risk) to 100 (high risk)
  name: risk_score
  type: integer
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/phone-intelligence-phone-intelligence-response-schema.json
slug: phone-intelligence-phone-intelligence-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/phone-intelligence-phone-intelligence-response-schema.json\",\n  \"title\": \"PhoneIntelligenceResponse\",\n  \"description\": \"Phone number intelligence response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number in E.164 format\",\n      \"example\": \"+14155552671\"\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the phone number is valid\",\n      \"example\": true\n    },\n    \"country\": {\n      \"$ref\": \"#/components/schemas/PhoneCountry\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic location of the phone number\",\n      \"example\": \"California\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Line type\",\n      \"example\": \"mobile\",\n      \"enum\": [\n        \"mobile\",\n        \"landline\",\n        \"voip\",\n        \"toll_free\",\n        \"premium_rate\",\n        \"shared_cost\",\n        \"unknown\"\n      ]\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier or service provider\",\n      \"example\": \"Verizon\"\n    },\n    \"is_voip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the number is a VoIP number\",\n      \"example\": false\n    },\n    \"risk_score\": {\n      \"type\": \"integer\",\n      \"description\": \"Risk score from 0 (low risk) to 100 (high risk)\",\n      \"example\": 12\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/phone-intelligence-phone-intelligence-response-schema.json
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
title: PhoneIntelligenceResponse
---
