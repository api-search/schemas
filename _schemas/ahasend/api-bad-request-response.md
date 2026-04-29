---
description: BadRequestResponse schema from AhaSend API
layout: schema
name: BadRequestResponse
properties_list:
- description: ''
  name: status
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-bad-request-response-schema.json
slug: api-bad-request-response
source_filename: api-bad-request-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-bad-request-response-schema.json\",\n  \"title\": \"BadRequestResponse\",\n  \"description\": \"BadRequestResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"domain is not yours\",\n        \"domain DNS config is not valid\"\n      ],\n      \"example\": \"example_value\"\n    }\n  },\n  \"example\": {\n    \"status\": \"bad request\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-bad-request-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: BadRequestResponse
---
