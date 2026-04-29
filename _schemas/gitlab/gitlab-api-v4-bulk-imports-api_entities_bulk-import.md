---
description: API_Entities_BulkImport model
layout: schema
name: API_Entities_BulkImport
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: source_type
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-import-schema.json
slug: gitlab-api-v4-bulk-imports-api_entities_bulk-import
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-import-schema.json\",\n  \"title\": \"API_Entities_BulkImport\",\n  \"description\": \"API_Entities_BulkImport model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"finished\",\n      \"enum\": [\n        \"created\",\n        \"started\",\n        \"finished\",\n        \"timeout\",\n        \"failed\"\n      ]\n    },\n    \"source_type\": {\n      \"type\": \"string\",\n      \"example\": \"gitlab\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28T11:42:42.000Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28T11:42:42.000Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-import-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_BulkImport
---
