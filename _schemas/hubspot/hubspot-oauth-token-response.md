---
description: Response containing the new access token and related information
layout: schema
name: TokenResponse
properties_list:
- description: The new access token
  name: access_token
  type: string
- description: The type of token (always 'bearer')
  name: token_type
  type: string
- description: Number of seconds until the access token expires
  name: expires_in
  type: integer
- description: The refresh token for obtaining new access tokens
  name: refresh_token
  type: string
- description: The ID token (only returned if openid scope was requested)
  name: id_token
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-oauth-token-response-schema.json
slug: hubspot-oauth-token-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response containing the new access token and related information\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The new access token\",\n      \"example\": \"CKDZpunPLhICAQEYs-gDIIGOBii1hQIyGQAf3xBKEgsYjYMJVvlHEz9tFHAwSq1TQAM40s0D\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of token (always 'bearer')\",\n      \"example\": \"bearer\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds until the access token expires\",\n      \"example\": 1800\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token for obtaining new access tokens\",\n      \"example\": \"6f18f26a-3e95-4d95-a6e5-3d5c6e5c9e5a\"\n    },\n    \"id_token\": {\n      \"type\": \"string\",\n      \"description\": \"The ID token (only returned if openid scope\
  \ was requested)\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...\"\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"token_type\",\n    \"expires_in\",\n    \"refresh_token\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-oauth-token-response-schema.json
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
title: TokenResponse
---
