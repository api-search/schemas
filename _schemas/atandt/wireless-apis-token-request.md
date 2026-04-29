---
description: OAuth 2.0 token request for AT&T Wireless APIs
layout: schema
name: Token Request
properties_list:
- description: ''
  name: grant_type
  type: string
- description: ''
  name: client_id
  type: string
- description: ''
  name: client_secret
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: refresh_token
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-token-request-schema.json
slug: wireless-apis-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/token-request\",\n  \"title\": \"Token Request\",\n  \"description\": \"OAuth 2.0 token request for AT&T Wireless APIs\",\n  \"type\": \"object\",\n  \"required\": [\n    \"grant_type\",\n    \"client_id\",\n    \"client_secret\",\n    \"scope\"\n  ],\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"client_credentials\",\n        \"authorization_code\",\n        \"refresh_token\"\n      ]\n    },\n    \"client_id\": {\n      \"type\": \"string\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\"\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-token-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Token Request
---
