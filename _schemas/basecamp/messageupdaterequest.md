---
description: ''
layout: schema
name: MessageUpdateRequest
properties_list:
- description: Updated message subject
  name: subject
  type: string
- description: Updated message body in HTML format
  name: content
  type: string
- description: Updated message category ID
  name: category_id
  type: integer
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/messageupdaterequest-schema.json
slug: messageupdaterequest
source_filename: messageupdaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/messageupdaterequest-schema.json\",\n  \"title\": \"MessageUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Updated message subject\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Updated message body in HTML format\"\n    },\n    \"category_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Updated message category ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/messageupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: MessageUpdateRequest
---
