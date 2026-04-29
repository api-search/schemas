---
description: The settings for attack payload logging.
layout: schema
name: attack-payload-logging
properties_list:
- description: Use `ATTACK_PAYLOAD` to log attack payloads for all requests, or use `NONE` if you don't want to log the attack payloads. Note that when set to `NONE`, you'll see `redacted` in the logging information
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-attack-payload-logging-schema.json
slug: api-security-attack-payload-logging
source_filename: api-security-attack-payload-logging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-attack-payload-logging-schema.json\",\n  \"title\": \"attack-payload-logging\",\n  \"description\": \"The settings for attack payload logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"Use `ATTACK_PAYLOAD` to log attack payloads for all requests, or use `NONE` if you don't want to log the attack payloads. Note that when set to `NONE`, you'll see `redacted` in the logging information instead of a blank space or sensitive information. For example, `JSON_PAIRS:redacted`.\",\n      \"enum\": [\n        \"ATTACK_PAYLOAD\",\n        \"NONE\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-attack-payload-logging-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: attack-payload-logging
---
