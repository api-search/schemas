---
description: ErrorResponse schema from Instagram Graph API
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: error
  type: object
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-error-response-schema.json
slug: instagram-graph-api-error-response
source_filename: instagram-graph-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"ErrorResponse schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"example\": \"Invalid OAuth access token.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"OAuthException\"\n        },\n        \"code\": {\n          \"type\": \"integer\",\n          \"example\": 190\n        },\n        \"fbtrace_id\": {\n          \"type\": \"string\",\n          \"example\": \"ABC123def456\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-error-response-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: ErrorResponse
---
