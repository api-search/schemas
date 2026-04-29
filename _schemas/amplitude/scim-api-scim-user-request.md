---
description: ScimUserRequest schema from Amplitude SCIM API
layout: schema
name: ScimUserRequest
properties_list:
- description: The SCIM schema URIs, typically urn:ietf:params:scim:schemas:core:2.0:User.
  name: schemas
  type: array
- description: The user's email address.
  name: userName
  type: string
- description: ''
  name: name
  type: object
- description: ''
  name: emails
  type: array
- description: Whether the user account should be active.
  name: active
  type: boolean
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-user-request-schema.json
slug: scim-api-scim-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-user-request-schema.json\",\n  \"title\": \"ScimUserRequest\",\n  \"description\": \"ScimUserRequest schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM schema URIs, typically urn:ietf:params:scim:schemas:core:2.0:User.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\"\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"givenName\": {\n          \"type\": \"string\",\n          \"description\": \"The user's first name.\"\n        },\n        \"familyName\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"The user's last name.\"\n        }\n      }\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"The email address.\"\n          },\n          \"primary\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this is the primary email.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of email.\"\n          }\n        }\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account should be active.\"\n    }\n  },\n  \"required\": [\n    \"schemas\",\n    \"userName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-user-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimUserRequest
---
