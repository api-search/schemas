---
description: Defines a `CLIENT_LIST` load shedding category for a URL protection policy.
layout: schema
name: url-protection-client-list-category
properties_list:
- description: A list of client list identifiers to match on.
  name: listIds
  type: array
- description: Whether the selected client lists match.
  name: positiveMatch
  type: boolean
- description: Specify `CLIENT_LIST` to match on a client list.
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-url-protection-client-list-category-schema.json
slug: api-security-url-protection-client-list-category
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-client-list-category-schema.json\",\n  \"title\": \"url-protection-client-list-category\",\n  \"description\": \"Defines a `CLIENT_LIST` load shedding category for a URL protection policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"listIds\": {\n      \"description\": \"A list of client list identifiers to match on.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"positiveMatch\": {\n      \"description\": \"Whether the selected client lists match.\",\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"description\": \"Specify `CLIENT_LIST` to match on a client list.\",\n      \"enum\": [\n        \"CLIENT_LIST\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\
  \n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-url-protection-client-list-category-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: url-protection-client-list-category
---
