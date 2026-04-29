---
description: Contains details of a security configuration.
layout: schema
name: config-rename
properties_list:
- description: Describes the security configuration.
  name: description
  type: string
- description: The name you assigned to the security configuration.
  name: name
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-config-rename-schema.json
slug: api-security-config-rename
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-rename-schema.json\",\n  \"title\": \"config-rename\",\n  \"description\": \"Contains details of a security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Describes the security configuration.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name you assigned to the security configuration.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-rename-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: config-rename
---
