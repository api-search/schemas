---
description: Contains match target settings and a list of objects containing match targets with their assigned sequence number.
layout: schema
name: match-targets-sequence
properties_list:
- description: Contains the ID and sequence of a match target.
  name: targetSequence
  type: array
- description: Describes the type of match target, either `WEBSITE` or `API`.
  name: type
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-match-targets-sequence-schema.json
slug: api-security-match-targets-sequence
source_filename: api-security-match-targets-sequence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-match-targets-sequence-schema.json\",\n  \"title\": \"match-targets-sequence\",\n  \"description\": \"Contains match target settings and a list of objects containing match targets with their assigned sequence number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetSequence\": {\n      \"description\": \"Contains the ID and sequence of a match target.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"sequence\": {\n            \"description\": \"The position in the sequence of match targets.\",\n            \"type\": \"integer\"\n          },\n          \"targetId\": {\n            \"description\": \"Uniquely identifies the match target.\",\n            \"type\": \"integer\"\n          }\n        },\n        \"required\"\
  : [\n          \"sequence\",\n          \"targetId\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"Describes the type of match target, either `WEBSITE` or `API`.\",\n      \"enum\": [\n        \"WEBSITE\",\n        \"API\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"targetSequence\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-match-targets-sequence-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: match-targets-sequence
---
