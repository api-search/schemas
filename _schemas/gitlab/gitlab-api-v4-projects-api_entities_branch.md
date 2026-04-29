---
description: API_Entities_Branch model
layout: schema
name: API_Entities_Branch
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: commit
  type: object
- description: ''
  name: merged
  type: boolean
- description: ''
  name: protected
  type: boolean
- description: ''
  name: developers_can_push
  type: boolean
- description: ''
  name: developers_can_merge
  type: boolean
- description: ''
  name: can_push
  type: boolean
- description: ''
  name: default
  type: boolean
- description: ''
  name: web_url
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-projects-api_entities_branch-schema.json
slug: gitlab-api-v4-projects-api_entities_branch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-projects-api_entities_branch-schema.json\",\n  \"title\": \"API_Entities_Branch\",\n  \"description\": \"API_Entities_Branch model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"master\"\n    },\n    \"commit\": {\n      \"$ref\": \"#/components/schemas/API_Entities_Commit\"\n    },\n    \"merged\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"protected\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"developers_can_push\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"developers_can_merge\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"can_push\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"default\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://gitlab.example.com/Commit921/the-dude/-/tree/master\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-projects-api_entities_branch-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Branch
---
