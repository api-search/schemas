---
description: Describes which headers you can exclude from inspection when you pass a `Pragma` debug header.
layout: schema
name: pragma-header
properties_list:
- description: The action to perform when a user passes a `Pragma` header. The only action currently supported is `REMOVE`.
  name: action
  type: string
- description: Use `OR` to match any condition, or `AND` to match on all conditions.
  name: conditionOperator
  type: string
- description: The conditions to exclude from the default `remove` action. Any condition you set in this object appears in the `Pragma` header debug response object.
  name: excludeCondition
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-pragma-header-schema.json
slug: api-security-pragma-header
source_filename: api-security-pragma-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-pragma-header-schema.json\",\n  \"title\": \"pragma-header\",\n  \"description\": \"Describes which headers you can exclude from inspection when you pass a `Pragma` debug header.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"The action to perform when a user passes a `Pragma` header. The only action currently supported is `REMOVE`.\",\n      \"enum\": [\n        \"REMOVE\"\n      ],\n      \"type\": \"string\"\n    },\n    \"conditionOperator\": {\n      \"description\": \"Use `OR` to match any condition, or `AND` to match on all conditions.\",\n      \"enum\": [\n        \"OR\",\n        \"AND\"\n      ],\n      \"type\": \"string\"\n    },\n    \"excludeCondition\": {\n      \"description\": \"The conditions to exclude from the default\
  \ `remove` action. Any condition you set in this object appears in the `Pragma` header debug response object.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"header\": {\n            \"description\": \"The name of the request header. In the example, `accept`.\",\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"The name of the request header to ignore from inspection. In the example, `type`.\",\n            \"type\": \"string\"\n          },\n          \"positiveMatch\": {\n            \"description\": \"When `true`, matches the selected values. When `false`, matches on anything outside the selected values.\",\n            \"type\": \"boolean\"\n          },\n          \"type\": {\n            \"description\": \"The header value you want to appear in the response. You can choose from `requestHeaderValueMatch`, `ipMatch`, `networkList`, or `queryParamNameValueMatch`.\",\n      \
  \      \"enum\": [\n              \"requestHeaderValueMatch\",\n              \"ipMatch\",\n              \"networkList\",\n              \"queryParamNameValueMatch\"\n            ],\n            \"type\": \"string\"\n          },\n          \"useHeaders\": {\n            \"description\": \"Whether the condition should include  the `X-Forwarded-For` header (XFF) header. This only applies when the condition `type` is `IP_MATCH` or `NETWORK_LIST`.\",\n            \"type\": \"boolean\"\n          },\n          \"value\": {\n            \"description\": \"List of header values, query parameter values, IP addresses, or names of network lists. To manage networks lists, use the [Network Lists API](https://techdocs.akamai.com/network-lists/reference/api).\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"type\": \"array\"\n          },\n          \"valueCase\": {\n            \"description\": \"Whether to consider the case-sensitivity of the provided\
  \ header value. This only applies when the condition `type` is `REQUEST_HEADER_VALUE_MATCH`.\",\n            \"type\": \"boolean\"\n          },\n          \"valueWildcard\": {\n            \"description\": \"Whether the provided header value includes wildcards, such as `*` or `?`. This only applies to the `REQUEST_HEADER_VALUE_MATCH` condition type.\",\n            \"type\": \"boolean\"\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"positiveMatch\",\n          \"value\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"action\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-pragma-header-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: pragma-header
---
