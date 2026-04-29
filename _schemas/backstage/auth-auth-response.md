---
description: AuthResponse schema from Backstage auth API
layout: schema
name: AuthResponse
properties_list:
- description: ''
  name: backstageIdentity
  type: object
- description: ''
  name: profile
  type: object
- description: ''
  name: providerInfo
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/auth-auth-response-schema.json
slug: auth-auth-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/auth-auth-response-schema.json\",\n  \"title\": \"AuthResponse\",\n  \"description\": \"AuthResponse schema from Backstage auth API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"backstageIdentity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"The Backstage token for backend API calls.\"\n        },\n        \"identity\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The identity type.\"\n            },\n            \"userEntityRef\": {\n              \"type\": \"string\",\n              \"description\": \"The entity reference for the user (e.g., user:default/guest).\"\n            },\n     \
  \       \"ownershipEntityRefs\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Entity references for groups and other ownership claims.\"\n            }\n          }\n        }\n      }\n    },\n    \"profile\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"description\": \"The user's email address.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The user's display name.\"\n        },\n        \"picture\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the user's profile picture.\"\n        }\n      }\n    },\n    \"providerInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"accessToken\": {\n          \"type\": \"string\",\n          \"description\": \"The provider-specific access token.\"\n     \
  \   },\n        \"expiresInSeconds\": {\n          \"type\": \"number\",\n          \"description\": \"Number of seconds until the access token expires.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/auth-auth-response-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: AuthResponse
---
