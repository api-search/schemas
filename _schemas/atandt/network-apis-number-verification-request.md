---
description: Request to verify a device phone number
layout: schema
name: Number Verification Request
properties_list:
- description: ''
  name: phoneNumber
  type: string
provider_name: AT&T
provider_slug: atandt
schema_file: json-schema/network-apis-number-verification-request-schema.json
slug: network-apis-number-verification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.att.com/schemas/network/number-verification-request\",\n  \"title\": \"Number Verification Request\",\n  \"description\": \"Request to verify a device phone number\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phoneNumber\"\n  ],\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+[1-9]\\\\d{1,14}$\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/json-schema/network-apis-number-verification-request-schema.json
tags:
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
title: Number Verification Request
---
