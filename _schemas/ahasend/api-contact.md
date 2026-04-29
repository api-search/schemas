---
description: Contact schema from AhaSend API
layout: schema
name: Contact
properties_list:
- description: ''
  name: email
  type: string
- description: ''
  name: name
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-contact-schema.json
slug: api-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"john@nasa.gov\",\n        \"jane@nasa.gov\"\n      ],\n      \"example\": \"user@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"John Smith\",\n        \"Jane Williams\"\n      ],\n      \"example\": \"Example Name\"\n    }\n  },\n  \"required\": [\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-contact-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Contact
---
