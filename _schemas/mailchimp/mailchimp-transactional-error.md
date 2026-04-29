---
description: A standard error response from the Mandrill API.
layout: schema
name: Error
properties_list:
- description: Always "error" for error responses.
  name: status
  type: string
- description: The numeric error code.
  name: code
  type: integer
- description: The name/type of the error (e.g., Invalid_Key, ValidationError).
  name: name
  type: string
- description: A human-readable description of the error.
  name: message
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-error-schema.json
slug: mailchimp-transactional-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"A standard error response from the Mandrill API.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Always \\\"error\\\" for error responses.\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The numeric error code.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name/type of the error (e.g., Invalid_Key, ValidationError).\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-error-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: Error
---
