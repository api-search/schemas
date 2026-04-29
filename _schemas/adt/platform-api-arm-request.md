---
description: Request to arm a security system.
layout: schema
name: ArmRequest
properties_list:
- description: Arming mode.
  name: mode
  type: string
- description: Valid access code to authorize arming.
  name: accessCode
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-arm-request-schema.json
slug: platform-api-arm-request
source_filename: platform-api-arm-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-arm-request-schema.json\",\n  \"title\": \"ArmRequest\",\n  \"description\": \"Request to arm a security system.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"mode\",\n    \"accessCode\"\n  ],\n  \"properties\": {\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"Arming mode.\",\n      \"enum\": [\n        \"away\",\n        \"stay\"\n      ],\n      \"example\": \"away\"\n    },\n    \"accessCode\": {\n      \"type\": \"string\",\n      \"description\": \"Valid access code to authorize arming.\",\n      \"example\": \"1234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-arm-request-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: ArmRequest
---
