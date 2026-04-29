---
description: Collects data needed for condition matches on request headers.
layout: schema
name: request-header-condition-2
properties_list:
- description: 'The type of condition. The `RequestHeaderCondition` type checks for a header from the requesting client and determines if it matches a provided header. This subtype supports the `?` wildcard to match '
  name: className
  type: string
- description: A header name. Use `name` to check whether the specified header exists.
  name: name
  type: array
- description: Whether to interpret `?` and `*` as wildcards.
  name: nameWildcard
  type: boolean
- description: Whether the condition triggers on a match or lack of match.
  name: positiveMatch
  type: boolean
- description: A list of unique header values. Use both `value` and `name` to check whether the requesting client’s header matches a provided header.
  name: value
  type: array
- description: Whether to consider the case sensitivity of the provided header values.
  name: valueCase
  type: boolean
- description: Whether to interpret `?` and `*` as wildcards.
  name: valueWildcard
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-request-header-condition-2-schema.json
slug: api-security-request-header-condition-2
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-request-header-condition-2-schema.json\",\n  \"title\": \"request-header-condition-2\",\n  \"description\": \"Collects data needed for condition matches on request headers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"className\": {\n      \"description\": \"The type of condition. The `RequestHeaderCondition` type checks for a header from the requesting client and determines if it matches a provided header. This subtype supports the `?` wildcard to match any single character and the `*` wildcard to match any sequence of 0 or more characters. You can also match on case sensitivity.\",\n      \"enum\": [\n        \"RequestHeaderCondition\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"A header name. Use `name` to check whether the specified\
  \ header exists.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"nameWildcard\": {\n      \"description\": \"Whether to interpret `?` and `*` as wildcards.\",\n      \"type\": \"boolean\"\n    },\n    \"positiveMatch\": {\n      \"description\": \"Whether the condition triggers on a match or lack of match.\",\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"description\": \"A list of unique header values. Use both `value` and `name` to check whether the requesting client\\u2019s header matches a provided header.\",\n      \"items\": {\n        \"minLength\": 1,\n        \"type\": \"string\"\n      },\n      \"nullable\": true,\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"valueCase\": {\n      \"description\": \"Whether to consider the case sensitivity of the provided header values.\",\n      \"type\": \"boolean\"\
  \n    },\n    \"valueWildcard\": {\n      \"description\": \"Whether to interpret `?` and `*` as wildcards.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"className\",\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-request-header-condition-2-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: request-header-condition-2
---
