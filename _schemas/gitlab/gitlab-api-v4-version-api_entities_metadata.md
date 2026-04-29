---
description: API_Entities_Metadata model
layout: schema
name: API_Entities_Metadata
properties_list:
- description: ''
  name: version
  type: string
- description: ''
  name: revision
  type: string
- description: ''
  name: kas
  type: object
- description: ''
  name: enterprise
  type: boolean
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-api-v4-version-api_entities_metadata-schema.json
slug: gitlab-api-v4-version-api_entities_metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-version-api_entities_metadata-schema.json\",\n  \"title\": \"API_Entities_Metadata\",\n  \"description\": \"API_Entities_Metadata model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"15.2-pre\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"example\": \"c401a659d0c\"\n    },\n    \"kas\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"externalUrl\": {\n          \"type\": \"string\",\n          \"example\": \"grpc://gitlab.example.com:8150\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"example\": \"15.0.0\"\n        }\n      }\n    },\n    \"enterprise\": {\n      \"type\": \"boolean\"\
  ,\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-api-v4-version-api_entities_metadata-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: API_Entities_Metadata
---
