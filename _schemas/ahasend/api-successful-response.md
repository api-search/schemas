---
description: SuccessfulResponse schema from AhaSend API
layout: schema
name: SuccessfulResponse
properties_list:
- description: Number of messages that were queued for sending.
  name: success_count
  type: integer
- description: Number of messages that failed to be queued for sending.
  name: fail_count
  type: integer
- description: List of email addresses that the email was not sent to.
  name: failed_recipients
  type: array
- description: ''
  name: errors
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-successful-response-schema.json
slug: api-successful-response
source_filename: api-successful-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-successful-response-schema.json\",\n  \"title\": \"SuccessfulResponse\",\n  \"description\": \"SuccessfulResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages that were queued for sending.\",\n      \"example\": 1\n    },\n    \"fail_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages that failed to be queued for sending.\",\n      \"example\": 1\n    },\n    \"failed_recipients\": {\n      \"type\": \"array\",\n      \"description\": \"List of email addresses that the email was not sent to.\",\n      \"example\": [\n        \"john@nasa.gov\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"errors\": {\n      \"\
  type\": \"array\",\n      \"example\": [\n        \"john@nasa.gov: The email account that you tried to reach does not exist.\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The reason the email failed to be sent to a recipient.\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-successful-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: SuccessfulResponse
---
