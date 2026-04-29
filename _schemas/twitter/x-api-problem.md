---
description: An HTTP Problem Details object, as defined in IETF RFC 7807 (https://tools.ietf.org/html/rfc7807).
layout: schema
name: Problem
properties_list:
- description: ''
  name: detail
  type: string
- description: ''
  name: status
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: type
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-problem-schema.json
slug: x-api-problem
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-problem-schema.json\",\n  \"title\": \"Problem\",\n  \"description\": \"An HTTP Problem Details object, as defined in IETF RFC 7807 (https://tools.ietf.org/html/rfc7807).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detail\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-problem-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Problem
---
