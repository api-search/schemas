---
description: ''
layout: schema
name: Campfire
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/campfire-schema.json
slug: campfire
source_filename: campfire-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/campfire-schema.json\",\n  \"title\": \"Campfire\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lines_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL to list campfire lines\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/campfire-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Campfire
---
