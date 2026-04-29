---
description: ''
layout: schema
name: Todo
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/todo-schema.json
slug: todo
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/todo-schema.json\",\n  \"title\": \"Todo\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"To-do text content\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted additional details\"\n        },\n        \"completed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this to-do has been completed\"\n        },\n        \"due_on\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Due date in ISO 8601 format\",\n          \"nullable\": true\n        },\n        \"starts_on\": {\n          \"type\": \"string\",\n          \"\
  format\": \"date\",\n          \"description\": \"Start date in ISO 8601 format\",\n          \"nullable\": true\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"Position within the to-do list\"\n        },\n        \"assignees\": {\n          \"type\": \"array\",\n          \"description\": \"People assigned to this to-do\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PersonRef\"\n          }\n        },\n        \"completion_subscribers\": {\n          \"type\": \"array\",\n          \"description\": \"People notified when this to-do is completed\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PersonRef\"\n          }\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this to-do\"\n        },\n        \"parent\": {\n          \"$ref\": \"#/components/schemas/Recording\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/todo-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Todo
---
