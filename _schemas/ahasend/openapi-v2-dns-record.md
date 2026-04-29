---
description: DNSRecord schema from AhaSend API
layout: schema
name: DNSRecord
properties_list:
- description: DNS record type (e.g., CNAME, TXT, MX)
  name: type
  type: string
- description: DNS record host/name
  name: host
  type: string
- description: DNS record content/value
  name: content
  type: string
- description: Whether this DNS record is required for domain verification
  name: required
  type: boolean
- description: Whether this DNS record has been propagated and verified
  name: propagated
  type: boolean
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-dns-record-schema.json
slug: openapi-v2-dns-record
source_filename: openapi-v2-dns-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-dns-record-schema.json\",\n  \"title\": \"DNSRecord\",\n  \"description\": \"DNSRecord schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"DNS record type (e.g., CNAME, TXT, MX)\",\n      \"example\": \"example_value\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"DNS record host/name\",\n      \"example\": \"example_value\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"DNS record content/value\",\n      \"example\": \"example_value\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this DNS record is required for domain verification\",\n      \"example\": true\n    },\n    \"propagated\": {\n \
  \     \"type\": \"boolean\",\n      \"description\": \"Whether this DNS record has been propagated and verified\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"host\",\n    \"content\",\n    \"required\",\n    \"propagated\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-dns-record-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DNSRecord
---
