---
description: ScimPatchRequest schema from Amplitude SCIM API
layout: schema
name: ScimPatchRequest
properties_list:
- description: The SCIM patch operation schema URI, typically urn:ietf:params:scim:api:messages:2.0:PatchOp.
  name: schemas
  type: array
- description: Array of patch operations to apply.
  name: Operations
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/scim-api-scim-patch-request-schema.json
slug: scim-api-scim-patch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-patch-request-schema.json\",\n  \"title\": \"ScimPatchRequest\",\n  \"description\": \"ScimPatchRequest schema from Amplitude SCIM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The SCIM patch operation schema URI, typically urn:ietf:params:scim:api:messages:2.0:PatchOp.\"\n    },\n    \"Operations\": {\n      \"type\": \"array\",\n      \"description\": \"Array of patch operations to apply.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"op\": {\n            \"type\": \"string\",\n            \"description\": \"The operation to perform.\",\n            \"enum\": [\n              \"add\",\n              \"remove\"\
  ,\n              \"replace\"\n            ]\n          },\n          \"path\": {\n            \"type\": \"string\",\n            \"description\": \"The attribute path to apply the operation to.\"\n          },\n          \"value\": {\n            \"description\": \"The value to use for the operation.\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"schemas\",\n    \"Operations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/scim-api-scim-patch-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: ScimPatchRequest
---
