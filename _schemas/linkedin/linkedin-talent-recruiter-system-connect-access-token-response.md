---
description: Response containing access token
layout: schema
name: AccessTokenResponse
properties_list:
- description: OAuth 2.0 access token
  name: access_token
  type: string
- description: Token expiration time in seconds
  name: expires_in
  type: integer
- description: Token type
  name: token_type
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-recruiter-system-connect-access-token-response-schema.json
slug: linkedin-talent-recruiter-system-connect-access-token-response
source_filename: linkedin-talent-recruiter-system-connect-access-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-access-token-response-schema.json\",\n  \"title\": \"AccessTokenResponse\",\n  \"description\": \"Response containing access token\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 access token\",\n      \"example\": \"AQV8vPRN5zF9BxJ...\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiration time in seconds\",\n      \"example\": 5184000\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type\",\n      \"example\": \"Bearer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-recruiter-system-connect-access-token-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AccessTokenResponse
---
