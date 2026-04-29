---
description: Risk assessment for the email
layout: schema
name: RiskInfo
properties_list:
- description: Risk level of the specific email address
  name: address_risk_status
  type: string
- description: Risk level of the domain
  name: domain_risk_status
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-risk-info-schema.json
slug: email-reputation-risk-info
source_filename: email-reputation-risk-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-risk-info-schema.json\",\n  \"title\": \"RiskInfo\",\n  \"description\": \"Risk assessment for the email\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address_risk_status\": {\n      \"type\": \"string\",\n      \"description\": \"Risk level of the specific email address\",\n      \"example\": \"low\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    },\n    \"domain_risk_status\": {\n      \"type\": \"string\",\n      \"description\": \"Risk level of the domain\",\n      \"example\": \"low\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-risk-info-schema.json
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
title: RiskInfo
---
