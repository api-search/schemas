---
description: Request body for obtaining access token
layout: schema
name: AccessTokenRequest
properties_list:
- description: ''
  name: grant_type
  type: string
- description: OAuth 2.0 client ID
  name: client_id
  type: string
- description: OAuth 2.0 client secret
  name: client_secret
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-access-token-request-schema.json
slug: linkedin-talent-recruiter-system-connect-access-token-request
source_filename: linkedin-talent-recruiter-system-connect-access-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-access-token-request-schema.json\",\n  \"title\": \"AccessTokenRequest\",\n  \"description\": \"Request body for obtaining access token\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"client_credentials\"\n      ],\n      \"example\": \"client_credentials\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client ID\",\n      \"example\": \"78abc123def456\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client secret\",\n      \"example\": \"secretXYZ789\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"client_id\",\n    \"client_secret\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-access-token-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AccessTokenRequest
---
