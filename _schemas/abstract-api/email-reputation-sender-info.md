---
description: Sender identity information
layout: schema
name: SenderInfo
properties_list:
- description: Inferred first name of sender
  name: first_name
  type: string
- description: Inferred last name of sender
  name: last_name
  type: string
- description: Name of the email provider
  name: email_provider_name
  type: string
- description: Organization associated with the email
  name: organization_name
  type: string
- description: Type of organization
  name: organization_type
  type: string
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/email-reputation-sender-info-schema.json
slug: email-reputation-sender-info
source_filename: email-reputation-sender-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-sender-info-schema.json\",\n  \"title\": \"SenderInfo\",\n  \"description\": \"Sender identity information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Inferred first name of sender\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Inferred last name of sender\",\n      \"example\": \"Smith\"\n    },\n    \"email_provider_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the email provider\",\n      \"example\": \"Google Workspace\"\n    },\n    \"organization_name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization associated with the email\",\n      \"example\": \"Example Corp\"\n    },\n    \"organization_type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Type of organization\",\n      \"example\": \"business\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/email-reputation-sender-info-schema.json
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
title: SenderInfo
---
