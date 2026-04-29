---
description: ''
layout: schema
name: TodoList
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/todolist-schema.json
slug: todolist
source_filename: todolist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/todolist-schema.json\",\n  \"title\": \"TodoList\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"completed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether all to-dos in this list are completed\"\n        },\n        \"completed_ratio\": {\n          \"type\": \"string\",\n          \"description\": \"Completion ratio as a string (e.g., \\\"2/5\\\")\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"Display position within the to-do set\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"List color identifier\",\n          \"nullable\": true\n        },\n        \"todos_url\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"uri\",\n          \"description\": \"API URL to list to-dos in this list\"\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this list\"\n        },\n        \"boosts_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of boosts on this list\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/todolist-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: TodoList
---
