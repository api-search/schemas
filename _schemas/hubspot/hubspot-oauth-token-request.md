---
description: Request body for token creation or refresh
layout: schema
name: TokenRequest
properties_list:
- description: The type of grant being requested
  name: grant_type
  type: string
- description: The client ID of your application
  name: client_id
  type: string
- description: The client secret of your application
  name: client_secret
  type: string
- description: The redirect URI (required for authorization_code grant)
  name: redirect_uri
  type: string
- description: The authorization code (required for authorization_code grant)
  name: code
  type: string
- description: The refresh token (required for refresh_token grant)
  name: refresh_token
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-oauth-token-request-schema.json
slug: hubspot-oauth-token-request
source_filename: hubspot-oauth-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for token creation or refresh\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of grant being requested\",\n      \"example\": \"refresh_token\",\n      \"enum\": [\n        \"authorization_code\",\n        \"refresh_token\"\n      ]\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The client ID of your application\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"The client secret of your application\",\n      \"example\": \"12345678-abcd-efgh-ijkl-9876543210ab\"\n    },\n    \"redirect_uri\": {\n      \"type\": \"string\",\n      \"description\": \"The redirect URI (required for authorization_code grant)\",\n      \"example\": \"https://myapp.example.com/oauth/callback\"\n    },\n    \"code\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The authorization code (required for authorization_code grant)\",\n      \"example\": \"abc123def456\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token (required for refresh_token grant)\",\n      \"example\": \"6f18f26a-3e95-4d95-a6e5-3d5c6e5c9e5a\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"client_id\",\n    \"client_secret\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-oauth-token-request-schema.json
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
title: TokenRequest
---
