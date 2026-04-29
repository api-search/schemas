---
description: Condition to be logged.
layout: schema
name: logging-option
properties_list:
- description: The unique identifier for each logging option. See [Logging option values](https://techdocs.akamai.com/application-security/reference/logging-option-values).
  name: id
  type: string
- description: A description of the logging option type.
  name: name
  type: string
- description: The value on which to match when determining whether to log the custom rule condition.
  name: value
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-logging-option-schema.json
slug: api-security-logging-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-logging-option-schema.json\",\n  \"title\": \"logging-option\",\n  \"description\": \"Condition to be logged.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The unique identifier for each logging option. See [Logging option values](https://techdocs.akamai.com/application-security/reference/logging-option-values).\",\n      \"enum\": [\n        \"CLIENT_TLS_FINGERPRINT_MATCH\",\n        \"HEADER_ORDER_MATCH\",\n        \"REQUEST_HEADER_MATCH\",\n        \"COOKIE_MATCH\",\n        \"URI_QUERY_MATCH\",\n        \"ARGS_POST_MATCH\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"A description of the logging option type.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The value\
  \ on which to match when determining whether to log the custom rule condition.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-logging-option-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: logging-option
---
