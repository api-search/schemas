---
description: UserId from LinkedIn API
layout: schema
name: UserId
properties_list:
- description: Type of user identifier
  name: idType
  type: string
- description: Hashed or identifier value
  name: idValue
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-user-id-schema.json
slug: linkedin-marketing-audience-user-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-user-id-schema.json\",\n  \"title\": \"UserId\",\n  \"description\": \"UserId from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"idType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SHA256_EMAIL\",\n        \"GOOGLE_AID\",\n        \"APPLE_IDFA\"\n      ],\n      \"description\": \"Type of user identifier\",\n      \"example\": \"SHA256_EMAIL\"\n    },\n    \"idValue\": {\n      \"type\": \"string\",\n      \"description\": \"Hashed or identifier value\",\n      \"example\": \"6b56c85c1ce461e7ef77e3a52f13a6bc09feb93a04ce0670f9909e8ffde01f3a\"\n    }\n  },\n  \"required\": [\n    \"idType\",\n    \"idValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-user-id-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: UserId
---
