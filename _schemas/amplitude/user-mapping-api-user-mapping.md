---
description: UserMapping schema from Amplitude User Mapping API
layout: schema
name: UserMapping
properties_list:
- description: The primary user ID that other identities will be mapped to.
  name: global_user_id
  type: string
- description: The user ID to map to the global_user_id.
  name: user_id
  type: string
- description: When true, removes the mapping instead of creating it.
  name: unmap
  type: boolean
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-mapping-api-user-mapping-schema.json
slug: user-mapping-api-user-mapping
source_filename: user-mapping-api-user-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-mapping-schema.json\",\n  \"title\": \"UserMapping\",\n  \"description\": \"UserMapping schema from Amplitude User Mapping API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"global_user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The primary user ID that other identities will be mapped to.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID to map to the global_user_id.\"\n    },\n    \"unmap\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, removes the mapping instead of creating it.\"\n    }\n  },\n  \"required\": [\n    \"global_user_id\",\n    \"user_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-mapping-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserMapping
---
