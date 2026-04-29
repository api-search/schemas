---
description: Reference to an image by upload ID or presigned URL.
layout: schema
name: ImageReference
properties_list:
- description: ''
  name: source
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-image-reference-schema.json
slug: adobe-firefly-api-image-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-image-reference-schema.json\",\n  \"title\": \"ImageReference\",\n  \"description\": \"Reference to an image by upload ID or presigned URL.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uploadId\": {\n          \"type\": \"string\",\n          \"description\": \"Upload ID from the image upload endpoint.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Presigned URL to the image.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-image-reference-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: ImageReference
---
