---
description: AccessDeniedResponse schema from AhaSend API
layout: schema
name: AccessDeniedResponse
properties_list:
- description: The reason your request failed.
  name: status
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-access-denied-response-schema.json
slug: api-access-denied-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-access-denied-response-schema.json\",\n  \"title\": \"AccessDeniedResponse\",\n  \"description\": \"AccessDeniedResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The reason your request failed.\",\n      \"examples\": [\n        \"invalid credentials\",\n        \"domain DNS config is not valid\"\n      ],\n      \"example\": \"example_value\"\n    }\n  },\n  \"example\": {\n    \"status\": \"invalid credentials\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-access-denied-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: AccessDeniedResponse
---
