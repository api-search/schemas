---
description: Email quality signals
layout: schema
name: EmailQuality
properties_list:
- description: Quality score from 0.0 to 1.0
  name: score
  type: number
- description: Whether the email is from a free provider
  name: is_free_email
  type: boolean
- description: Whether the username appears suspicious
  name: is_username_suspicious
  type: boolean
- description: Whether the email is from a disposable provider
  name: is_disposable
  type: boolean
- description: Whether the domain accepts all emails
  name: is_catchall
  type: boolean
- description: Whether the email uses a subaddress (+ tag)
  name: is_subaddress
  type: boolean
- description: Whether the email is a role-based address
  name: is_role
  type: boolean
- description: Whether DMARC policy is enforced
  name: is_dmarc_enforced
  type: boolean
- description: Whether SPF is strictly enforced
  name: is_spf_strict
  type: boolean
- description: Minimum estimated age of the email in days
  name: minimum_age
  type: integer
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-email-quality-schema.json
slug: email-reputation-email-quality
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-email-quality-schema.json\",\n  \"title\": \"EmailQuality\",\n  \"description\": \"Email quality signals\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Quality score from 0.0 to 1.0\",\n      \"example\": 0.92\n    },\n    \"is_free_email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is from a free provider\",\n      \"example\": false\n    },\n    \"is_username_suspicious\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the username appears suspicious\",\n      \"example\": false\n    },\n    \"is_disposable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is from a disposable provider\",\n      \"example\"\
  : false\n    },\n    \"is_catchall\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain accepts all emails\",\n      \"example\": false\n    },\n    \"is_subaddress\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email uses a subaddress (+ tag)\",\n      \"example\": false\n    },\n    \"is_role\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is a role-based address\",\n      \"example\": false\n    },\n    \"is_dmarc_enforced\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether DMARC policy is enforced\",\n      \"example\": true\n    },\n    \"is_spf_strict\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SPF is strictly enforced\",\n      \"example\": false\n    },\n    \"minimum_age\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum estimated age of the email in days\",\n      \"example\": 365\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-email-quality-schema.json
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
title: EmailQuality
---
