---
description: Recipient schema from AhaSend API
layout: schema
name: Recipient
properties_list:
- description: Recipient email address
  name: email
  type: string
- description: Display name for the recipient
  name: name
  type: string
- description: Substitution data for the recipient. Used with jinja2 templating language for dynamic content
  name: substitutions
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-recipient-schema.json
slug: openapi-v2-recipient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-recipient-schema.json\",\n  \"title\": \"Recipient\",\n  \"description\": \"Recipient schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Recipient email address\",\n      \"example\": \"user@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the recipient\",\n      \"example\": \"Example Name\"\n    },\n    \"substitutions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Substitution data for the recipient. Used with jinja2 templating language for dynamic content\",\n      \"example\": {}\n    }\n  },\n  \"required\": [\n    \"email\"\n  ],\n  \"example\": {\n    \"email\"\
  : \"user@example.com\",\n    \"name\": \"John Doe\",\n    \"substitutions\": {\n      \"first_name\": \"John\",\n      \"order_id\": \"12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-recipient-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Recipient
---
