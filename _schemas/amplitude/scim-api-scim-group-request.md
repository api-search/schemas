---
description: ScimGroupRequest schema from Amplitude SCIM API
layout: schema
name: ScimGroupRequest
properties_list:
- description: The SCIM schema URIs.
  name: schemas
  type: array
- description: The display name of the group.
  name: displayName
  type: string
- description: Array of initial group members.
  name: members
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-group-request-schema.json
slug: scim-api-scim-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-request-schema.json\",\n  \"title\": \"ScimGroupRequest\",\n  \"description\": \"ScimGroupRequest schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM schema URIs.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the group.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Array of initial group members.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The member user ID.\"\n          }\n        }\n      }\n\
  \    }\n  },\n  \"required\": [\n    \"schemas\",\n    \"displayName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimGroupRequest
---
