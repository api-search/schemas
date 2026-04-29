---
description: NumberVerificationRequest schema
layout: schema
name: NumberVerificationRequest
properties_list:
- description: Phone number in E.164 format to verify against the requesting device
  name: phoneNumber
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/number-verification-api-number-verification-request-schema.json
slug: number-verification-api-number-verification-request
source_filename: number-verification-api-number-verification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/number-verification-api-number-verification-request-schema.json\",\n  \"title\": \"NumberVerificationRequest\",\n  \"description\": \"NumberVerificationRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phoneNumber\"\n  ],\n  \"properties\": {\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number in E.164 format to verify against the requesting device\",\n      \"example\": \"+12125551234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/json-schema/number-verification-api-number-verification-request-schema.json
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: NumberVerificationRequest
---
