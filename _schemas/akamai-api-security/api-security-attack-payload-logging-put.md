---
description: The PUT Request JSON for attack payload logging.
layout: schema
name: attack-payload-logging-put
properties_list:
- description: Whether attack payload logging is enabled.
  name: enabled
  type: boolean
- description: Settings for request body.
  name: requestBody
  type: object
- description: Settings for response body.
  name: responseBody
  type: object
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-attack-payload-logging-put-schema.json
slug: api-security-attack-payload-logging-put
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-attack-payload-logging-put-schema.json\",\n  \"title\": \"attack-payload-logging-put\",\n  \"description\": \"The PUT Request JSON for attack payload logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"Whether attack payload logging is enabled.\",\n      \"type\": \"boolean\"\n    },\n    \"requestBody\": {\n      \"additionalProperties\": false,\n      \"description\": \"Settings for request body.\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"Use `ATTACK_PAYLOAD` to log attack payloads for all requests, or use `NONE` if you don't want to log the attack payloads. Note that when set to `NONE`, you'll see `redacted` in the logging information instead of a blank space or sensitive information. For example,\
  \ `JSON_PAIRS:redacted`.\",\n          \"enum\": [\n            \"ATTACK_PAYLOAD\",\n            \"NONE\"\n          ],\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/attack-payload-logging.yaml\"\n      }\n    },\n    \"responseBody\": {\n      \"additionalProperties\": false,\n      \"description\": \"Settings for response body.\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"Use `ATTACK_PAYLOAD` to log attack payloads for all requests, or use `NONE` if you don't want to log the attack payloads. Note that when set to `NONE`, you'll see `redacted` in the logging information instead of a blank space or sensitive information. For example, `JSON_PAIRS:redacted`.\",\n          \"enum\": [\n            \"ATTACK_PAYLOAD\",\n            \"NONE\"\n          ],\n          \"type\": \"string\"\n        }\n      },\n      \"\
  required\": [\n        \"type\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/attack-payload-logging.yaml\"\n      }\n    }\n  },\n  \"required\": [\n    \"enabled\",\n    \"requestBody\",\n    \"responseBody\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-attack-payload-logging-put-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: attack-payload-logging-put
---
