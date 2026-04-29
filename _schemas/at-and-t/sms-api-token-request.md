---
description: TokenRequest schema from AT&T API
layout: schema
name: TokenRequest
properties_list:
- description: The App Key from your AT&T developer account
  name: client_id
  type: string
- description: The App Secret from your AT&T developer account
  name: client_secret
  type: string
- description: OAuth grant type
  name: grant_type
  type: string
- description: Space-separated list of API scopes (e.g. SMS, MMS, SPEECH)
  name: scope
  type: string
- description: Authorization code (required for authorization_code grant type)
  name: code
  type: string
- description: Refresh token (required for refresh_token grant type)
  name: refresh_token
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-token-request-schema.json
slug: sms-api-token-request
source_filename: sms-api-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-token-request-schema.json\",\n  \"title\": \"TokenRequest\",\n  \"description\": \"TokenRequest schema from AT&T API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"client_id\",\n    \"client_secret\",\n    \"grant_type\",\n    \"scope\"\n  ],\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The App Key from your AT&T developer account\",\n      \"example\": \"your_app_key\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"The App Secret from your AT&T developer account\",\n      \"example\": \"your_app_secret\"\n    },\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth grant type\",\n      \"enum\": [\n        \"client_credentials\",\n        \"authorization_code\",\n      \
  \  \"refresh_token\"\n      ],\n      \"example\": \"client_credentials\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Space-separated list of API scopes (e.g. SMS, MMS, SPEECH)\",\n      \"example\": \"SMS\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization code (required for authorization_code grant type)\",\n      \"example\": \"auth_code_abc123\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token (required for refresh_token grant type)\",\n      \"example\": \"f6e5d4c3b2a1f6e5d4c3b2a1f6e5d4c3\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-token-request-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TokenRequest
---
