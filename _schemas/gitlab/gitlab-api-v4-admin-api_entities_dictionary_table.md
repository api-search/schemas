---
description: API_Entities_Dictionary_Table model
layout: schema
name: API_Entities_Dictionary_Table
properties_list:
- description: ''
  name: table_name
  type: string
- description: ''
  name: feature_categories
  type: array
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-admin-api_entities_dictionary_table-schema.json
slug: gitlab-api-v4-admin-api_entities_dictionary_table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_dictionary_table-schema.json\",\n  \"title\": \"API_Entities_Dictionary_Table\",\n  \"description\": \"API_Entities_Dictionary_Table model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"table_name\": {\n      \"type\": \"string\",\n      \"example\": \"users\"\n    },\n    \"feature_categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"database\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-admin-api_entities_dictionary_table-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Dictionary_Table
---
