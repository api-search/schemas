---
description: ''
layout: schema
name: Document
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/document-schema.json
slug: document
source_filename: document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/document-schema.json\",\n  \"title\": \"Document\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted document body\"\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this document\"\n        },\n        \"boosts_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of boosts on this document\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"Display position within the vault\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/document-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Document
---
