---
description: Contains details about an overlapping configuration.
layout: schema
name: overlap-config
properties_list:
- description: The configuration ID.
  name: configId
  type: integer
- description: The configuration name.
  name: configName
  type: string
- description: The configuration version.
  name: configVersion
  type: integer
- description: The contract ID.
  name: contractId
  type: string
- description: The contract name.
  name: contractName
  type: string
- description: List of version tags, any combination of `STAGING` and `LAST_CREATED`.
  name: hostnames
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-overlap-config-schema.json
slug: api-security-overlap-config
source_filename: api-security-overlap-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-overlap-config-schema.json\",\n  \"title\": \"overlap-config\",\n  \"description\": \"Contains details about an overlapping configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configId\": {\n      \"description\": \"The configuration ID.\",\n      \"type\": \"integer\"\n    },\n    \"configName\": {\n      \"description\": \"The configuration name.\",\n      \"type\": \"string\"\n    },\n    \"configVersion\": {\n      \"description\": \"The configuration version.\",\n      \"type\": \"integer\"\n    },\n    \"contractId\": {\n      \"description\": \"The contract ID.\",\n      \"type\": \"string\"\n    },\n    \"contractName\": {\n      \"description\": \"The contract name.\",\n      \"type\": \"string\"\n    },\n    \"hostnames\": {\n      \"description\": \"List of\
  \ version tags, any combination of `STAGING` and `LAST_CREATED`.\",\n      \"items\": {\n        \"description\": \"The version tag.\",\n        \"enum\": [\n          \"STAGING\",\n          \"LAST_CREATED\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"configId\",\n    \"configName\",\n    \"configVersion\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-overlap-config-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: overlap-config
---
