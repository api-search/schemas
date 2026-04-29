---
description: ScimUserListResponse schema from Amplitude SCIM API
layout: schema
name: ScimUserListResponse
properties_list:
- description: The SCIM schema URIs for this response.
  name: schemas
  type: array
- description: The total number of matching users.
  name: totalResults
  type: integer
- description: The 1-based index of the first result.
  name: startIndex
  type: integer
- description: The number of results returned in this page.
  name: itemsPerPage
  type: integer
- description: Array of SCIM user resources.
  name: Resources
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-user-list-response-schema.json
slug: scim-api-scim-user-list-response
source_filename: scim-api-scim-user-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-user-list-response-schema.json\",\n  \"title\": \"ScimUserListResponse\",\n  \"description\": \"ScimUserListResponse schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM schema URIs for this response.\"\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of matching users.\"\n    },\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The 1-based index of the first result.\"\n    },\n    \"itemsPerPage\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned in this page.\"\n    },\n    \"Resources\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Array of SCIM user resources.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"schemas\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"The SCIM schema URIs for this resource.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The SCIM unique identifier for the user.\"\n          },\n          \"userName\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"The user's email address, used as the primary identifier.\"\n          },\n          \"name\": {\n            \"type\": \"object\",\n            \"description\": \"The user's name components.\",\n            \"properties\": {\n              \"givenName\": {\n                \"type\": \"string\",\n                \"description\": \"The user's first\
  \ name.\"\n              },\n              \"familyName\": {\n                \"type\": \"string\",\n                \"description\": \"The user's last name.\"\n              }\n            }\n          },\n          \"emails\": {\n            \"type\": \"array\",\n            \"description\": \"Array of email addresses for the user.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"format\": \"email\",\n                  \"description\": \"The email address.\"\n                },\n                \"primary\": {\n                  \"type\": \"boolean\",\n                  \"description\": \"Whether this is the primary email address.\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"description\": \"The type of email address such as work or personal.\"\n                }\n             \
  \ }\n            }\n          },\n          \"active\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the user account is active.\"\n          },\n          \"groups\": {\n            \"type\": \"array\",\n            \"description\": \"Array of groups the user belongs to.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The group ID.\"\n                },\n                \"display\": {\n                  \"type\": \"string\",\n                  \"description\": \"The group display name.\"\n                }\n              }\n            }\n          },\n          \"meta\": {\n            \"type\": \"object\",\n            \"description\": \"SCIM metadata for the resource.\",\n            \"properties\": {\n              \"resourceType\": {\n                \"type\": \"string\",\n                \"\
  description\": \"The type of SCIM resource.\"\n              },\n              \"created\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"The date and time the resource was created.\"\n              },\n              \"lastModified\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"The date and time the resource was last modified.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-user-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimUserListResponse
---
