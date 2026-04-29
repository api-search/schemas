---
description: UpdateAccountRequest schema from AhaSend API
layout: schema
name: UpdateAccountRequest
properties_list:
- description: Account name
  name: name
  type: string
- description: Account website URL
  name: website
  type: string
- description: Account description (used for account verification)
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
schema_file: json-schema/openapi-v2-update-account-request-schema.json
slug: openapi-v2-update-account-request
source_filename: openapi-v2-update-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-account-request-schema.json\",\n  \"title\": \"UpdateAccountRequest\",\n  \"description\": \"UpdateAccountRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Account name\",\n      \"example\": \"Example Name\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Account website URL\",\n      \"example\": \"https://example.com\"\n    },\n    \"about\": {\n      \"type\": \"string\",\n      \"description\": \"Account description (used for account verification)\",\n      \"example\": \"example_value\"\n    },\n    \"track_opens\": {\n      \"type\": \"boolean\",\n      \"description\": \"Default open tracking setting\"\
  ,\n      \"example\": true\n    },\n    \"track_clicks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Default click tracking setting\",\n      \"example\": true\n    },\n    \"reject_bad_recipients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to reject bad recipients\",\n      \"example\": true\n    },\n    \"reject_mistyped_recipients\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to reject mistyped recipients\",\n      \"example\": true\n    },\n    \"message_metadata_retention\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 30,\n      \"description\": \"Default message metadata retention in days\",\n      \"example\": 1\n    },\n    \"message_data_retention\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 30,\n      \"description\": \"Default message data retention in days\",\n      \"example\": 1\n    }\n  },\n  \"example\": {\n    \"name\": \"Updated Company Name\"\
  ,\n    \"website\": \"https://example.com\",\n    \"track_opens\": true\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-account-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: UpdateAccountRequest
---
