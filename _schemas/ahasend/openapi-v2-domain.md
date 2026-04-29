---
description: Domain schema from AhaSend API
layout: schema
name: Domain
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the domain
  name: id
  type: string
- description: When the domain was created
  name: created_at
  type: string
- description: When the domain was last updated
  name: updated_at
  type: string
- description: The domain name
  name: domain
  type: string
- description: Account ID this domain belongs to
  name: account_id
  type: string
- description: DNS records required for domain verification
  name: dns_records
  type: array
- description: When DNS records were last checked
  name: last_dns_check_at
  type: string
- description: Whether all required DNS records are properly configured
  name: dns_valid
  type: boolean
- description: Custom tracking subdomain. Null means the account or product default is used.
  name: tracking_subdomain
  type: string
- description: Custom return-path subdomain. Null means the account or product default is used.
  name: return_path_subdomain
  type: string
- description: Custom subscription management subdomain. Null means the account or product default is used.
  name: subscription_subdomain
  type: string
- description: Custom media subdomain. Null means the account or product default is used.
  name: media_subdomain
  type: string
- description: Custom DKIM rotation interval in days. Null means the account default is used.
  name: dkim_rotation_interval_days
  type: integer
- description: Whether the standby DKIM slot is ready for rotation.
  name: rotation_ready
  type: boolean
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-domain-schema.json
slug: openapi-v2-domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-domain-schema.json\",\n  \"title\": \"Domain\",\n  \"description\": \"Domain schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"domain\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"domain\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the domain\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the domain was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"When the domain was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name\",\n      \"example\": \"mail.example.com\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Account ID this domain belongs to\",\n      \"example\": \"500123\"\n    },\n    \"dns_records\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DNSRecord\"\n      },\n      \"description\": \"DNS records required for domain verification\",\n      \"example\": [\n        {\n          \"type\": \"example_value\",\n          \"host\": \"example_value\",\n          \"content\": \"example_value\",\n          \"required\": true,\n          \"propagated\": true\n        }\n      ]\n    },\n    \"last_dns_check_at\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"format\": \"date-time\",\n   \
  \   \"description\": \"When DNS records were last checked\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"dns_valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether all required DNS records are properly configured\",\n      \"example\": true\n    },\n    \"tracking_subdomain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Custom tracking subdomain. Null means the account or product default is used.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"return_path_subdomain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Custom return-path subdomain. Null means the account or product default is used.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"subscription_subdomain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Custom subscription management subdomain. Null means the account or product default is used.\",\n      \"\
  example\": \"mail.example.com\"\n    },\n    \"media_subdomain\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Custom media subdomain. Null means the account or product default is used.\",\n      \"example\": \"mail.example.com\"\n    },\n    \"dkim_rotation_interval_days\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Custom DKIM rotation interval in days. Null means the account default is used.\",\n      \"example\": 1\n    },\n    \"rotation_ready\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the standby DKIM slot is ready for rotation.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"domain\",\n    \"account_id\",\n    \"dns_records\",\n    \"dns_valid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-domain-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Domain
---
