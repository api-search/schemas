---
description: SalesAccessToken from LinkedIn API
layout: schema
name: SalesAccessToken
properties_list:
- description: Short-lived, limited-scope OAuth token
  name: token
  type: string
- description: Time at which this token will become invalid (seconds since epoch)
  name: expiryTime
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-sales-access-token-schema.json
slug: linkedin-sales-navigator-sales-access-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-access-token-schema.json\",\n  \"title\": \"SalesAccessToken\",\n  \"description\": \"SalesAccessToken from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Short-lived, limited-scope OAuth token\",\n      \"example\": \"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...\"\n    },\n    \"expiryTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which this token will become invalid (seconds since epoch)\",\n      \"example\": 1640100000\n    }\n  },\n  \"required\": [\n    \"token\",\n    \"expiryTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-access-token-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SalesAccessToken
---
