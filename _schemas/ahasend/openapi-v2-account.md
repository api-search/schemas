---
description: Account schema from AhaSend API
layout: schema
name: Account
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the account
  name: id
  type: string
- description: When the account was created
  name: created_at
  type: string
- description: When the account was last updated
  name: updated_at
  type: string
- description: Account name
  name: name
  type: string
- description: Account website URL
  name: website
  type: string
- description: Account description
  name: about
  type: string
- description: Default open tracking setting
  name: track_opens
  type: boolean
- description: Default click tracking setting
  name: track_clicks
  type: boolean
- description: Whether to reject bad recipients
  name: reject_bad_recipients
  type: boolean
- description: Whether to reject mistyped recipients
  name: reject_mistyped_recipients
  type: boolean
- description: Default message metadata retention in days
  name: message_metadata_retention
  type: integer
- description: Default message data retention in days
  name: message_data_retention
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-account-schema.json
slug: openapi-v2-account
source_filename: openapi-v2-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"Account schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"account\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"account\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the account\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the account was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"When the account was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name\",\n      \"example\": \"Example Name\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"Account website URL\",\n      \"example\": \"https://example.com\"\n    },\n    \"about\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Account description\",\n      \"example\": \"example_value\"\n    },\n    \"track_opens\": {\n      \"type\": \"boolean\",\n      \"description\": \"Default open tracking setting\",\n      \"example\": true\n    },\n    \"track_clicks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Default click tracking setting\",\n      \"example\": true\n    },\n    \"reject_bad_recipients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ to reject bad recipients\",\n      \"example\": true\n    },\n    \"reject_mistyped_recipients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to reject mistyped recipients\",\n      \"example\": true\n    },\n    \"message_metadata_retention\": {\n      \"type\": \"integer\",\n      \"description\": \"Default message metadata retention in days\",\n      \"example\": 1\n    },\n    \"message_data_retention\": {\n      \"type\": \"integer\",\n      \"description\": \"Default message data retention in days\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-account-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Account
---
