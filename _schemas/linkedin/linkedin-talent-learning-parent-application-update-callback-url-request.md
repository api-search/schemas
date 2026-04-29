---
description: Request body for updating OAuth 2.0 callback URLs
layout: schema
name: UpdateCallbackUrlRequest
properties_list:
- description: ''
  name: patch
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-learning-parent-application-update-callback-url-request-schema.json
slug: linkedin-talent-learning-parent-application-update-callback-url-request
source_filename: linkedin-talent-learning-parent-application-update-callback-url-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-update-callback-url-request-schema.json\",\n  \"title\": \"UpdateCallbackUrlRequest\",\n  \"description\": \"Request body for updating OAuth 2.0 callback URLs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patch\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"$set\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"oauth2AuthorizedCallbackUrls\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\n              },\n              \"example\": [\n                \"https://app.acme.com/oauth2/callback\",\n                \"https://new-domain.acme.com/oauth2/callback\"\n              ]\n            }\n          }\n     \
  \   }\n      }\n    }\n  },\n  \"required\": [\n    \"patch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-learning-parent-application-update-callback-url-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: UpdateCallbackUrlRequest
---
