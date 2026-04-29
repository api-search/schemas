---
description: A user's permission for a given repository.
layout: schema
name: repository_permission
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: permission
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-user-repository_permission-schema.json
slug: atlassian-bitbucket-user-repository_permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"repository_permission\",\n  \"type\": \"object\",\n  \"description\": \"A user's permission for a given repository.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"permission\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-user-repository_permission-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: repository_permission
---
