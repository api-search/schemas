---
description: Full IP intelligence response
layout: schema
name: IPIntelligenceResponse
properties_list:
- description: Analyzed IP address
  name: ip_address
  type: string
- description: ''
  name: security
  type: object
- description: ''
  name: asn
  type: object
- description: ''
  name: company
  type: object
- description: Known domains associated with this IP
  name: domains
  type: array
- description: ''
  name: location
  type: object
- description: ''
  name: timezone
  type: object
- description: ''
  name: flag
  type: object
- description: ''
  name: currency
  type: object
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-intelligence-ip-intelligence-response-schema.json
slug: ip-intelligence-ip-intelligence-response
source_filename: ip-intelligence-ip-intelligence-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-ip-intelligence-response-schema.json\",\n  \"title\": \"IPIntelligenceResponse\",\n  \"description\": \"Full IP intelligence response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"Analyzed IP address\",\n      \"example\": \"8.8.8.8\"\n    },\n    \"security\": {\n      \"$ref\": \"#/components/schemas/IPSecurityFlags\"\n    },\n    \"asn\": {\n      \"$ref\": \"#/components/schemas/ASNInfo\"\n    },\n    \"company\": {\n      \"$ref\": \"#/components/schemas/CompanyBasic\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"Known domains associated with this IP\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"dns.google\"\n      ]\n\
  \    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/LocationInfo\"\n    },\n    \"timezone\": {\n      \"$ref\": \"#/components/schemas/TimezoneInfo\"\n    },\n    \"flag\": {\n      \"$ref\": \"#/components/schemas/FlagInfo\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/components/schemas/CurrencyInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-ip-intelligence-response-schema.json
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
title: IPIntelligenceResponse
---
