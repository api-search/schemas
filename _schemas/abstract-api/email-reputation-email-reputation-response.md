---
description: Email reputation and validation response
layout: schema
name: EmailReputationResponse
properties_list:
- description: The email address analyzed
  name: email
  type: string
- description: ''
  name: deliverability
  type: object
- description: ''
  name: quality
  type: object
- description: ''
  name: sender
  type: object
- description: ''
  name: domain
  type: object
- description: ''
  name: risk
  type: object
- description: ''
  name: breaches
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-email-reputation-response-schema.json
slug: email-reputation-email-reputation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-email-reputation-response-schema.json\",\n  \"title\": \"EmailReputationResponse\",\n  \"description\": \"Email reputation and validation response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address analyzed\",\n      \"example\": \"test@example.com\"\n    },\n    \"deliverability\": {\n      \"$ref\": \"#/components/schemas/Deliverability\"\n    },\n    \"quality\": {\n      \"$ref\": \"#/components/schemas/EmailQuality\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/components/schemas/SenderInfo\"\n    },\n    \"domain\": {\n      \"$ref\": \"#/components/schemas/DomainInfo\"\n    },\n    \"risk\": {\n      \"$ref\": \"#/components/schemas/RiskInfo\"\n    },\n    \"breaches\"\
  : {\n      \"$ref\": \"#/components/schemas/BreachInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-email-reputation-response-schema.json
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
title: EmailReputationResponse
---
