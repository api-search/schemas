---
description: Email schema from AhaSend API
layout: schema
name: Email
properties_list:
- description: ''
  name: from
  type: object
- description: Specifies the list of recipients to which message will be sent.
  name: recipients
  type: array
- description: ''
  name: content
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-email-schema.json
slug: api-email
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-email-schema.json\",\n  \"title\": \"Email\",\n  \"description\": \"Email schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"$ref\": \"#/components/schemas/Contact\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the list of recipients to which message will be sent.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Contact\"\n      },\n      \"example\": [\n        {\n          \"email\": \"user@example.com\",\n          \"name\": \"Example Name\"\n        }\n      ]\n    },\n    \"content\": {\n      \"$ref\": \"#/components/schemas/Content\"\n    }\n  },\n  \"required\": [\n    \"from\",\n    \"recipients\",\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-email-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Email
---
