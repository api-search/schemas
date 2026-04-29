---
description: Request to disarm a security system.
layout: schema
name: DisarmRequest
properties_list:
- description: Valid access code to authorize disarming.
  name: accessCode
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-disarm-request-schema.json
slug: platform-api-disarm-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-disarm-request-schema.json\",\n  \"title\": \"DisarmRequest\",\n  \"description\": \"Request to disarm a security system.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"accessCode\"\n  ],\n  \"properties\": {\n    \"accessCode\": {\n      \"type\": \"string\",\n      \"description\": \"Valid access code to authorize disarming.\",\n      \"example\": \"1234\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-disarm-request-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: DisarmRequest
---
