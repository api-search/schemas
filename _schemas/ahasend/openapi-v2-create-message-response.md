---
description: CreateMessageResponse schema from AhaSend API
layout: schema
name: CreateMessageResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: List of messages and their statuses
  name: data
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-message-response-schema.json
slug: openapi-v2-create-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-message-response-schema.json\",\n  \"title\": \"CreateMessageResponse\",\n  \"description\": \"CreateMessageResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CreateSingleMessageResponse\"\n      },\n      \"description\": \"List of messages and their statuses\",\n      \"example\": [\n        {\n          \"object\": \"message\",\n          \"id\": \"500123\",\n          \"recipient\": {},\n          \"status\": \"queued\",\n          \"error\": \"example_value\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-message-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateMessageResponse
---
