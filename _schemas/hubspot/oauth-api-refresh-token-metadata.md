---
description: Metadata associated with an OAuth refresh token
layout: schema
name: RefreshTokenMetadata
properties_list:
- description: The refresh token string
  name: token
  type: string
- description: The client ID of the application
  name: client_id
  type: string
- description: The HubSpot portal (hub) ID associated with this token
  name: hub_id
  type: integer
- description: The ID of the user who authorized the token
  name: user_id
  type: integer
- description: The email address of the user who authorized the token
  name: user
  type: string
- description: List of scopes granted to this token
  name: scopes
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/oauth-api-refresh-token-metadata-schema.json
slug: oauth-api-refresh-token-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/oauth-api-refresh-token-metadata-schema.json\",\n  \"title\": \"RefreshTokenMetadata\",\n  \"description\": \"Metadata associated with an OAuth refresh token\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token string\",\n      \"example\": \"6f18f26a-3e95-4d95-a6e5-3d5c6e5c9e5a\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The client ID of the application\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"hub_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The HubSpot portal (hub) ID associated with this token\",\n      \"example\": 62515\n    },\n    \"user_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user\
  \ who authorized the token\",\n      \"example\": 123456\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who authorized the token\",\n      \"example\": \"user@example.com\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"List of scopes granted to this token\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"contacts\",\n        \"content\"\n      ]\n    }\n  },\n  \"required\": [\n    \"token\",\n    \"client_id\",\n    \"hub_id\",\n    \"scopes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/oauth-api-refresh-token-metadata-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: RefreshTokenMetadata
---
