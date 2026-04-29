---
description: Address schema from AhaSend API
layout: schema
name: Address
properties_list:
- description: Valid email address from a domain defined in your account with valid DNS records
  name: email
  type: string
- description: Display name for the sender
  name: name
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-address-schema.json
slug: openapi-v2-address
source_filename: openapi-v2-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Valid email address from a domain defined in your account with valid DNS records\",\n      \"example\": \"user@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the sender\",\n      \"example\": \"Example Name\"\n    }\n  },\n  \"required\": [\n    \"email\"\n  ],\n  \"example\": {\n    \"email\": \"noreply@example.com\",\n    \"name\": \"Example Corp\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-address-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Address
---
