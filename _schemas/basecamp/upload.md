---
description: ''
layout: schema
name: Upload
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/upload-schema.json
slug: upload
source_filename: upload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/upload-schema.json\",\n  \"title\": \"Upload\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"Original filename of the upload\"\n        },\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the file\"\n        },\n        \"byte_size\": {\n          \"type\": \"integer\",\n          \"description\": \"File size in bytes\"\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Image width in pixels (for image files)\",\n          \"nullable\": true\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Image height in pixels\
  \ (for image files)\",\n          \"nullable\": true\n        },\n        \"download_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Direct download URL for the file\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted upload description\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"Display position within the vault\"\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this upload\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/upload-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Upload
---
