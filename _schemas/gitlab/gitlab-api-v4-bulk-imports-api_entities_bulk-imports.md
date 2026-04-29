---
description: API_Entities_BulkImports model
layout: schema
name: API_Entities_BulkImports
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: bulk_import_id
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: entity_type
  type: string
- description: ''
  name: source_full_path
  type: string
- description: ''
  name: destination_full_path
  type: string
- description: ''
  name: destination_name
  type: string
- description: ''
  name: destination_slug
  type: string
- description: ''
  name: destination_namespace
  type: string
- description: ''
  name: parent_id
  type: integer
- description: ''
  name: namespace_id
  type: integer
- description: ''
  name: project_id
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: failures
  type: array
- description: ''
  name: migrate_projects
  type: boolean
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-imports-schema.json
slug: gitlab-api-v4-bulk-imports-api_entities_bulk-imports
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-imports-schema.json\",\n  \"title\": \"API_Entities_BulkImports\",\n  \"description\": \"API_Entities_BulkImports model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"bulk_import_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"created\",\n      \"enum\": [\n        \"created\",\n        \"started\",\n        \"finished\",\n        \"timeout\",\n        \"failed\"\n      ]\n    },\n    \"entity_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"group\",\n        \"project\"\n      ],\n      \"example\": \"group\"\n    },\n\
  \    \"source_full_path\": {\n      \"type\": \"string\",\n      \"example\": \"source_group\"\n    },\n    \"destination_full_path\": {\n      \"type\": \"string\",\n      \"example\": \"some_group/source_project\"\n    },\n    \"destination_name\": {\n      \"type\": \"string\",\n      \"example\": \"destination_slug\"\n    },\n    \"destination_slug\": {\n      \"type\": \"string\",\n      \"example\": \"destination_slug\"\n    },\n    \"destination_namespace\": {\n      \"type\": \"string\",\n      \"example\": \"destination_path\"\n    },\n    \"parent_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"namespace_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28T11:42:42.000Z\"\
  \n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2012-05-28T11:42:42.000Z\"\n    },\n    \"failures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/API_Entities_BulkImports_EntityFailure\"\n      }\n    },\n    \"migrate_projects\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-bulk-imports-api_entities_bulk-imports-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_BulkImports
---
