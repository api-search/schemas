---
description: A SCIM 2.0 user resource for provisioning users into the Torii platform.
layout: schema
name: Torii SCIM User
properties_list:
- description: ''
  name: schemas
  type: array
- description: Unique SCIM identifier.
  name: id
  type: string
- description: Username, typically the email address.
  name: userName
  type: string
- description: ''
  name: name
  type: object
- description: ''
  name: emails
  type: array
- description: Whether the user is active.
  name: active
  type: boolean
- description: Display name.
  name: displayName
  type: string
- description: External identifier from the identity provider.
  name: externalId
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/scim-user.json
slug: scim-user
source_filename: scim-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/scim-user.json\",\n  \"title\": \"Torii SCIM User\",\n  \"description\": \"A SCIM 2.0 user resource for provisioning users into the Torii platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"urn:ietf:params:scim:schemas:core:2.0:User\"]\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique SCIM identifier.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Username, typically the email address.\"\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"givenName\": {\n          \"type\": \"string\",\n          \"description\": \"First name.\"\n        },\n   \
  \     \"familyName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name.\"\n        }\n      }\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"primary\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is active.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name.\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External identifier from the identity provider.\"\n    }\n  },\n  \"required\": [\"userName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/scim-user.json
tags:
- SaaS Management
title: Torii SCIM User
---
