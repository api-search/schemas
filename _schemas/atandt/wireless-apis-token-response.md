---
description: OAuth 2.0 token response from AT&T
layout: schema
name: Token Response
properties_list:
- description: ''
  name: access_token
  type: string
- description: ''
  name: token_type
  type: string
- description: ''
  name: expires_in
  type: integer
- description: ''
  name: refresh_token
  type: string
- description: ''
  name: scope
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/wireless-apis-token-response-schema.json
slug: wireless-apis-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/wireless/token-response\",\n  \"title\": \"Token Response\",\n  \"description\": \"OAuth 2.0 token response from AT&T\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"bearer\"\n      ]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\"\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/wireless-apis-token-response-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Token Response
---
