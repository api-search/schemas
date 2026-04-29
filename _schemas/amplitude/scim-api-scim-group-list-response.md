---
description: ScimGroupListResponse schema from Amplitude SCIM API
layout: schema
name: ScimGroupListResponse
properties_list:
- description: The SCIM schema URIs for this response.
  name: schemas
  type: array
- description: The total number of matching groups.
  name: totalResults
  type: integer
- description: Array of SCIM group resources.
  name: Resources
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-group-list-response-schema.json
slug: scim-api-scim-group-list-response
source_filename: scim-api-scim-group-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-list-response-schema.json\",\n  \"title\": \"ScimGroupListResponse\",\n  \"description\": \"ScimGroupListResponse schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM schema URIs for this response.\"\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of matching groups.\"\n    },\n    \"Resources\": {\n      \"type\": \"array\",\n      \"description\": \"Array of SCIM group resources.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"schemas\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\"\
  : \"string\"\n            },\n            \"description\": \"The SCIM schema URIs for this resource.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The SCIM unique identifier for the group.\"\n          },\n          \"displayName\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the group.\"\n          },\n          \"members\": {\n            \"type\": \"array\",\n            \"description\": \"Array of group members.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The member user ID.\"\n                },\n                \"display\": {\n                  \"type\": \"string\",\n                  \"description\": \"The member display name.\"\n                }\n              }\n            }\n          },\n          \"meta\": {\n\
  \            \"type\": \"object\",\n            \"description\": \"SCIM metadata for the resource.\",\n            \"properties\": {\n              \"resourceType\": {\n                \"type\": \"string\",\n                \"description\": \"The type of SCIM resource.\"\n              },\n              \"created\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"The date and time the resource was created.\"\n              },\n              \"lastModified\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"The date and time the resource was last modified.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-group-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimGroupListResponse
---
