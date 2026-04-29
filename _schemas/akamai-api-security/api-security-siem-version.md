---
description: Contains Security Information Event Management (SIEM) version settings.
layout: schema
name: siem-version
properties_list:
- description: Uniquely identifies the SIEM version.
  name: id
  type: integer
- description: The name assigned to the SIEM version.
  name: name
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-siem-version-schema.json
slug: api-security-siem-version
source_filename: api-security-siem-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-version-schema.json\",\n  \"title\": \"siem-version\",\n  \"description\": \"Contains Security Information Event Management (SIEM) version settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Uniquely identifies the SIEM version.\",\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"description\": \"The name assigned to the SIEM version.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-version-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: siem-version
---
