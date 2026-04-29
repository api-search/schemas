---
description: CreateSingleMessageResponse schema from AhaSend API
layout: schema
name: CreateSingleMessageResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Message ID (null if the message was not sent)
  name: id
  type: string
- description: ''
  name: recipient
  type: object
- description: Status of the message
  name: status
  type: string
- description: Error message if the message was not sent
  name: error
  type: string
- description: Provided if the request contained a schedule
  name: schedule
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-single-message-response-schema.json
slug: openapi-v2-create-single-message-response
source_filename: openapi-v2-create-single-message-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-single-message-response-schema.json\",\n  \"title\": \"CreateSingleMessageResponse\",\n  \"description\": \"CreateSingleMessageResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"message\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"message\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Message ID (null if the message was not sent)\",\n      \"example\": \"<uuid@example.com>\"\n    },\n    \"recipient\": {\n      \"$ref\": \"#/components/schemas/Recipient\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"queued\",\n        \"scheduled\",\n        \"error\"\
  \n      ],\n      \"description\": \"Status of the message\",\n      \"example\": \"queued\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Error message if the message was not sent\",\n      \"example\": \"example_value\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/components/schemas/MessageSchedule\",\n      \"description\": \"Provided if the request contained a schedule\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"recipient\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-single-message-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateSingleMessageResponse
---
