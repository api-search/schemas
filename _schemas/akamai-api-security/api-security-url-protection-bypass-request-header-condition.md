---
description: Collects data needed for condition matches on request headers.
layout: schema
name: url-protection-bypass-request-header-condition
properties_list:
- description: Choose `RequestHeaderCondition` to match a header from the requesting client to the specified header.
  name: className
  type: string
- description: Use `name` to check whether the specified header exists.
  name: name
  type: array
- description: Whether to interpret `?` and `*` as wildcards in the specified `name`.
  name: nameWildcard
  type: boolean
- description: __Read-only__ Whether the condition triggers on a match or lack of match.
  name: positiveMatch
  type: boolean
- description: A list of unique header values. Use both `value` and `name` to check whether the requesting client’s header matches the specified headers.
  name: value
  type: array
- description: Whether to consider case when matching header values, `true` for case-sensitive matches.
  name: valueCase
  type: boolean
- description: Whether to interpret `?` and `*` as wildcards in the specified `value`.
  name: valueWildcard
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-bypass-request-header-condition-schema.json
slug: api-security-url-protection-bypass-request-header-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-bypass-request-header-condition-schema.json\",\n  \"title\": \"url-protection-bypass-request-header-condition\",\n  \"description\": \"Collects data needed for condition matches on request headers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"className\": {\n      \"description\": \"Choose `RequestHeaderCondition` to match a header from the requesting client to the specified header.\",\n      \"enum\": [\n        \"RequestHeaderCondition\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Use `name` to check whether the specified header exists.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n\
  \    \"nameWildcard\": {\n      \"description\": \"Whether to interpret `?` and `*` as wildcards in the specified `name`.\",\n      \"type\": \"boolean\"\n    },\n    \"positiveMatch\": {\n      \"description\": \"__Read-only__ Whether the condition triggers on a match or lack of match.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"description\": \"A list of unique header values. Use both `value` and `name` to check whether the requesting client\\u2019s header matches the specified headers.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"nullable\": true,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"valueCase\": {\n      \"description\": \"Whether to consider case when matching header values, `true` for case-sensitive matches.\",\n      \"type\": \"boolean\"\n    },\n    \"valueWildcard\": {\n      \"description\": \"Whether to interpret `?` and `*` as wildcards\
  \ in the specified `value`.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"className\",\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-bypass-request-header-condition-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-bypass-request-header-condition
---
