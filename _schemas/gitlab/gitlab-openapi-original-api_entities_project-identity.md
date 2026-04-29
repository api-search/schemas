---
description: API_Entities_ProjectIdentity from GitLab API
layout: schema
name: API_Entities_ProjectIdentity
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: description
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: name_with_namespace
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: path_with_namespace
  type: string
- description: ''
  name: created_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-openapi-original-api_entities_project-identity-schema.json
slug: gitlab-openapi-original-api_entities_project-identity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_project-identity-schema.json\",\n  \"title\": \"API_Entities_ProjectIdentity\",\n  \"description\": \"API_Entities_ProjectIdentity from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"example\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"desc\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"project1\"\n    },\n    \"name_with_namespace\": {\n      \"type\": \"string\",\n      \"example\": \"John Doe / project1\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"example\": \"project1\"\n    },\n    \"path_with_namespace\": {\n      \"type\": \"string\",\n      \"example\": \"namespace1/project1\"\n\
  \    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2020-05-07 04:27:17.016000+00:00\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-openapi-original-api_entities_project-identity-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_ProjectIdentity
---
