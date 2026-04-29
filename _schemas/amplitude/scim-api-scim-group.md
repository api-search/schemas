---
description: ScimGroup schema from Amplitude SCIM API
layout: schema
name: ScimGroup
properties_list:
- description: The SCIM schema URIs for this resource.
  name: schemas
  type: array
- description: The SCIM unique identifier for the group.
  name: id
  type: string
- description: The display name of the group.
  name: displayName
  type: string
- description: Array of group members.
  name: members
  type: array
- description: SCIM metadata for the resource.
  name: meta
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-group-schema.json
slug: scim-api-scim-group
source_filename: scim-api-scim-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-schema.json\",\n  \"title\": \"ScimGroup\",\n  \"description\": \"ScimGroup schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM schema URIs for this resource.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The SCIM unique identifier for the group.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the group.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Array of group members.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"\
  type\": \"string\",\n            \"description\": \"The member user ID.\"\n          },\n          \"display\": {\n            \"type\": \"string\",\n            \"description\": \"The member display name.\"\n          }\n        }\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"SCIM metadata for the resource.\",\n      \"properties\": {\n        \"resourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of SCIM resource.\"\n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the resource was created.\"\n        },\n        \"lastModified\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the resource was last modified.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimGroup
---
