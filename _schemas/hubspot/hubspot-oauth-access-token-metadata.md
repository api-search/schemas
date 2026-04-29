---
description: Metadata associated with an OAuth access token
layout: schema
name: AccessTokenMetadata
properties_list:
- description: The access token string
  name: token
  type: string
- description: The ID of the HubSpot application associated with this token
  name: app_id
  type: integer
- description: The HubSpot portal (hub) ID associated with this token
  name: hub_id
  type: integer
- description: The ID of the user who authorized the token
  name: user_id
  type: integer
- description: The email address of the user who authorized the token
  name: user
  type: string
- description: The domain of the HubSpot portal
  name: hub_domain
  type: string
- description: List of scopes granted to this token
  name: scopes
  type: array
- description: The type of token (always 'access')
  name: token_type
  type: string
- description: Number of seconds until the token expires
  name: expires_in
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-oauth-access-token-metadata-schema.json
slug: hubspot-oauth-access-token-metadata
source_filename: hubspot-oauth-access-token-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata associated with an OAuth access token\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token string\",\n      \"example\": \"CKDZpunPLhICAQEYs-gDIIGOBii1hQIyGQAf3xBKEgsYjYMJVvlHEz9tFHAwSq1TQAM40s0D\"\n    },\n    \"app_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the HubSpot application associated with this token\",\n      \"example\": 456789\n    },\n    \"hub_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The HubSpot portal (hub) ID associated with this token\",\n      \"example\": 62515\n    },\n    \"user_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user who authorized the token\",\n      \"example\": 123456\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who authorized the token\",\n      \"example\": \"user@example.com\"\
  \n    },\n    \"hub_domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain of the HubSpot portal\",\n      \"example\": \"demo.hubspot.com\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"description\": \"List of scopes granted to this token\",\n      \"example\": [\n        \"contacts\",\n        \"content\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of token (always 'access')\",\n      \"example\": \"access\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds until the token expires\",\n      \"example\": 1800\n    }\n  },\n  \"required\": [\n    \"token\",\n    \"app_id\",\n    \"hub_id\",\n    \"scopes\",\n    \"token_type\",\n    \"expires_in\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessTokenMetadata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-oauth-access-token-metadata-schema.json
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
title: AccessTokenMetadata
---
