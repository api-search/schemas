---
description: Contains details about SIEM versions.
layout: schema
name: siem-versions
properties_list:
- description: A list of SIEM versions.
  name: siemDefinitions
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-siem-versions-schema.json
slug: api-security-siem-versions
source_filename: api-security-siem-versions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-versions-schema.json\",\n  \"title\": \"siem-versions\",\n  \"description\": \"Contains details about SIEM versions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"siemDefinitions\": {\n      \"description\": \"A list of SIEM versions.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains Security Information Event Management (SIEM) version settings.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Uniquely identifies the SIEM version.\",\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"description\": \"The name assigned to the SIEM version.\",\n            \"type\": \"boolean\"\n          }\n        },\n        \"required\": [\n          \"id\",\n     \
  \     \"name\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/siem-version.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-versions-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: siem-versions
---
