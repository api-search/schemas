---
description: ''
layout: schema
name: UploadUpdateRequest
properties_list:
- description: Revised upload description in HTML format
  name: description
  type: string
- description: New filename without extension
  name: base_name
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/uploadupdaterequest-schema.json
slug: uploadupdaterequest
source_filename: uploadupdaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/uploadupdaterequest-schema.json\",\n  \"title\": \"UploadUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Revised upload description in HTML format\"\n    },\n    \"base_name\": {\n      \"type\": \"string\",\n      \"description\": \"New filename without extension\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/uploadupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: UploadUpdateRequest
---
