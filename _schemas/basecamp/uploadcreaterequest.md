---
description: ''
layout: schema
name: UploadCreateRequest
properties_list:
- description: Signed global ID of the attachment obtained from the Basecamp attachment API
  name: attachable_sgid
  type: string
- description: HTML-formatted information about the upload
  name: description
  type: string
- description: Filename without extension
  name: base_name
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/uploadcreaterequest-schema.json
slug: uploadcreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/uploadcreaterequest-schema.json\",\n  \"title\": \"UploadCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"attachable_sgid\"\n  ],\n  \"properties\": {\n    \"attachable_sgid\": {\n      \"type\": \"string\",\n      \"description\": \"Signed global ID of the attachment obtained from the Basecamp attachment API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted information about the upload\"\n    },\n    \"base_name\": {\n      \"type\": \"string\",\n      \"description\": \"Filename without extension\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/uploadcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: UploadCreateRequest
---
