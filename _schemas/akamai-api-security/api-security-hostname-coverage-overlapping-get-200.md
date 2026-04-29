---
description: Describes configurations that use the same hostname, causing overlapping coverage.
layout: schema
name: hostname-coverage-overlapping-get-200
properties_list:
- description: The list of configurations that overlap coverage for the hostname.
  name: overLappingList
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-hostname-coverage-overlapping-get-200-schema.json
slug: api-security-hostname-coverage-overlapping-get-200
source_filename: api-security-hostname-coverage-overlapping-get-200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-coverage-overlapping-get-200-schema.json\",\n  \"title\": \"hostname-coverage-overlapping-get-200\",\n  \"description\": \"Describes configurations that use the same hostname, causing overlapping coverage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"overLappingList\": {\n      \"description\": \"The list of configurations that overlap coverage for the hostname.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains details about an overlapping configuration.\",\n        \"properties\": {\n          \"configId\": {\n            \"description\": \"The configuration ID.\",\n            \"type\": \"integer\"\n          },\n          \"configName\": {\n            \"description\": \"The configuration name.\",\n            \"\
  type\": \"string\"\n          },\n          \"configVersion\": {\n            \"description\": \"The configuration version.\",\n            \"type\": \"integer\"\n          },\n          \"contractId\": {\n            \"description\": \"The contract ID.\",\n            \"type\": \"string\"\n          },\n          \"contractName\": {\n            \"description\": \"The contract name.\",\n            \"type\": \"string\"\n          },\n          \"hostnames\": {\n            \"description\": \"List of version tags, any combination of `STAGING` and `LAST_CREATED`.\",\n            \"items\": {\n              \"description\": \"The version tag.\",\n              \"enum\": [\n                \"STAGING\",\n                \"LAST_CREATED\"\n              ],\n              \"type\": \"string\"\n            },\n            \"type\": \"array\"\n          }\n        },\n        \"required\": [\n          \"configId\",\n          \"configName\",\n          \"configVersion\"\n        ],\n        \"\
  type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/overlap-config.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"overLappingList\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-coverage-overlapping-get-200-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: hostname-coverage-overlapping-get-200
---
