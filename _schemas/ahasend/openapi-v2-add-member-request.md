---
description: AddMemberRequest schema from AhaSend API
layout: schema
name: AddMemberRequest
properties_list:
- description: Email address of the user to add
  name: email
  type: string
- description: Display name for the user
  name: name
  type: string
- description: Role to assign to the user
  name: role
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-add-member-request-schema.json
slug: openapi-v2-add-member-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-add-member-request-schema.json\",\n  \"title\": \"AddMemberRequest\",\n  \"description\": \"AddMemberRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user to add\",\n      \"example\": \"user@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the user\",\n      \"example\": \"Example Name\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Administrator\",\n        \"Developer\",\n        \"Analyst\",\n        \"Billing Manager\"\n      ],\n      \"description\": \"Role to assign to the user\",\n      \"example\": \"Administrator\"\n    }\n  },\n  \"required\"\
  : [\n    \"email\",\n    \"role\"\n  ],\n  \"example\": {\n    \"email\": \"user@example.com\",\n    \"name\": \"John Doe\",\n    \"role\": \"Developer\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-add-member-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: AddMemberRequest
---
