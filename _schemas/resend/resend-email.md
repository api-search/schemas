---
description: JSON Schema for a Resend email object as returned by the /emails/{id} endpoint.
layout: schema
name: Resend Email
properties_list:
- description: The type of object.
  name: object
  type: string
- description: The ID of the email.
  name: id
  type: string
- description: The email addresses of the recipients.
  name: to
  type: array
- description: The email address of the sender.
  name: from
  type: string
- description: The date and time the email was created.
  name: created_at
  type: string
- description: The subject line of the email.
  name: subject
  type: string
- description: The HTML body of the email.
  name: html
  type:
  - string
  - 'null'
- description: The plain text body of the email.
  name: text
  type:
  - string
  - 'null'
- description: Blind carbon copy recipients.
  name: bcc
  type:
  - array
  - 'null'
- description: Carbon copy recipients.
  name: cc
  type:
  - array
  - 'null'
- description: Reply-to addresses.
  name: reply_to
  type:
  - array
  - 'null'
- description: The status of the email.
  name: last_event
  type: string
provider_name: Resend
provider_slug: resend
schema_file: json-schema/resend-email-schema.json
slug: resend-email
source_filename: resend-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/resend/json-schema/resend-email-schema.json\",\n  \"title\": \"Resend Email\",\n  \"description\": \"JSON Schema for a Resend email object as returned by the /emails/{id} endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"email\",\n      \"description\": \"The type of object.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the email.\",\n      \"example\": \"4ef9a417-02e9-4d39-ad75-9611e0fcc33c\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"The email addresses of the recipients.\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the sender.\",\n      \"example\": \"Acme <onboarding@resend.dev>\"\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the email was created.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject line of the email.\"\n    },\n    \"html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The HTML body of the email.\"\n    },\n    \"text\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The plain text body of the email.\"\n    },\n    \"bcc\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Blind carbon copy recipients.\"\n    },\n    \"cc\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Carbon copy recipients.\"\n    },\n    \"reply_to\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Reply-to addresses.\"\n    },\n  \
  \  \"last_event\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the email.\",\n      \"example\": \"delivered\"\n    }\n  },\n  \"required\": [\"id\", \"from\", \"to\", \"subject\", \"created_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/json-schema/resend-email-schema.json
tags:
- Email
- Developer Tools
- Transactional Email
- Marketing Email
title: Resend Email
---
