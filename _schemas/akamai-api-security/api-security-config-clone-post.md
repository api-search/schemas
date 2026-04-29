---
description: Specifies the settings for a new clone of a security configuration.
layout: schema
name: config-clone-post
properties_list:
- description: The configuration version to clone from.
  name: createFromVersion
  type: integer
- description: Specifies whether the application rules should be migrated to the latest version.
  name: ruleUpdate
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-config-clone-post-schema.json
slug: api-security-config-clone-post
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-clone-post-schema.json\",\n  \"title\": \"config-clone-post\",\n  \"description\": \"Specifies the settings for a new clone of a security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createFromVersion\": {\n      \"description\": \"The configuration version to clone from.\",\n      \"type\": \"integer\"\n    },\n    \"ruleUpdate\": {\n      \"description\": \"Specifies whether the application rules should be migrated to the latest version.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"createFromVersion\",\n    \"ruleUpdate\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-config-clone-post-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: config-clone-post
---
