---
description: The header settings for HTTP Header Logging.
layout: schema
name: logging-header-setting
properties_list:
- description: 'Use `all` to log headers for all requests with any standard header. Use `none` to exclude headers for any requests with any standard header from logging. Use `exclude` to exclude headers for requests '
  name: type
  type: string
- description: List of headers to include or exclude depending on the `type` setting.
  name: values
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-logging-header-setting-schema.json
slug: api-security-logging-header-setting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-logging-header-setting-schema.json\",\n  \"title\": \"logging-header-setting\",\n  \"description\": \"The header settings for HTTP Header Logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"Use `all` to log headers for all requests with any standard header. Use `none` to exclude headers for any requests with any standard header from logging. Use `exclude` to exclude headers for requests with specific standard headers. Use `only` to include headers for requests with specific standard headers.\",\n      \"enum\": [\n        \"all\",\n        \"none\",\n        \"exclude\",\n        \"only\"\n      ],\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"description\": \"List of headers to include or exclude depending on the `type`\
  \ setting.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-logging-header-setting-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: logging-header-setting
---
