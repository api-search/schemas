---
description: API_Entities_BatchedBackgroundMigration model
layout: schema
name: API_Entities_BatchedBackgroundMigration
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: job_class_name
  type: string
- description: ''
  name: table_name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: progress
  type: number
- description: ''
  name: created_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-admin-api_entities_batched-background-migration-schema.json
slug: gitlab-api-v4-admin-api_entities_batched-background-migration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_batched-background-migration-schema.json\",\n  \"title\": \"API_Entities_BatchedBackgroundMigration\",\n  \"description\": \"API_Entities_BatchedBackgroundMigration model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"1234\"\n    },\n    \"job_class_name\": {\n      \"type\": \"string\",\n      \"example\": \"CopyColumnUsingBackgroundMigrationJob\"\n    },\n    \"table_name\": {\n      \"type\": \"string\",\n      \"example\": \"events\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 50\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"example\": \"2022-11-28T14:26:39.000Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_batched-background-migration-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_BatchedBackgroundMigration
---
