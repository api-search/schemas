---
description: Content schema from AhaSend API
layout: schema
name: Content
properties_list:
- description: ''
  name: subject
  type: string
- description: Plaintext body of the email
  name: text_body
  type: string
- description: HTML body of the email
  name: html_body
  type: string
- description: ''
  name: attachments
  type: array
- description: ''
  name: reply_to
  type: object
- description: Specify arbitary headers.
  name: headers
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-content-schema.json
slug: api-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-content-schema.json\",\n  \"title\": \"Content\",\n  \"description\": \"Content schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"Sample subject\"\n      ],\n      \"example\": \"example_value\"\n    },\n    \"text_body\": {\n      \"type\": \"string\",\n      \"description\": \"Plaintext body of the email\",\n      \"examples\": [\n        \"Sample email body\"\n      ],\n      \"example\": \"example_value\"\n    },\n    \"html_body\": {\n      \"type\": \"string\",\n      \"description\": \"HTML body of the email\",\n      \"examples\": [\n        \"<p>Sample email body</p>\"\n      ],\n      \"example\": \"example_value\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\":\
  \ {\n        \"$ref\": \"#/components/schemas/Attachment\"\n      },\n      \"example\": [\n        {\n          \"data\": \"example_value\",\n          \"base64\": true,\n          \"content_type\": \"example_value\",\n          \"content_id\": \"500123\",\n          \"file_name\": \"Example Name\"\n        }\n      ]\n    },\n    \"reply_to\": {\n      \"$ref\": \"#/components/schemas/Contact\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Specify arbitary headers.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"X-My-Mail-ID\": \"12345\",\n        \"X-Comment-ID\": \"456789\"\n      }\n    }\n  },\n  \"required\": [\n    \"subject\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-content-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Content
---
