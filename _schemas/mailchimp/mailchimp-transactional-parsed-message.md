---
description: A parsed MIME message.
layout: schema
name: ParsedMessage
properties_list:
- description: The parsed subject line.
  name: subject
  type: string
- description: The parsed sender email address.
  name: from_email
  type: string
- description: The parsed sender name.
  name: from_name
  type: string
- description: Parsed recipient list.
  name: to
  type: array
- description: All parsed headers.
  name: headers
  type: object
- description: The plain-text body.
  name: text
  type: string
- description: The HTML body.
  name: html
  type: string
- description: Parsed file attachments.
  name: attachments
  type: array
- description: Parsed inline images.
  name: images
  type: array
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-parsed-message-schema.json
slug: mailchimp-transactional-parsed-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParsedMessage\",\n  \"type\": \"object\",\n  \"description\": \"A parsed MIME message.\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The parsed subject line.\"\n    },\n    \"from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The parsed sender email address.\"\n    },\n    \"from_name\": {\n      \"type\": \"string\",\n      \"description\": \"The parsed sender name.\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"description\": \"Parsed recipient list.\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"All parsed headers.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The plain-text body.\"\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML body.\"\n    },\n    \"attachments\": {\n      \"type\": \"\
  array\",\n      \"description\": \"Parsed file attachments.\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"Parsed inline images.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-parsed-message-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: ParsedMessage
---
