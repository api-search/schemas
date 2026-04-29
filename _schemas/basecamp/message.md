---
description: ''
layout: schema
name: Message
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/message-schema.json
slug: message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/message-schema.json\",\n  \"title\": \"Message\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"subject\": {\n          \"type\": \"string\",\n          \"description\": \"Message subject/title\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted message body\"\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this message\"\n        },\n        \"comments_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL to list comments\"\n        },\n        \"boosts_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number\
  \ of boosts (reactions) on this message\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/message-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Message
---
