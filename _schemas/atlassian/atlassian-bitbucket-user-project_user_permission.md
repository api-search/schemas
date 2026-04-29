---
description: A user's direct permission for a given project.
layout: schema
name: project_user_permission
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: permission
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-user-project_user_permission-schema.json
slug: atlassian-bitbucket-user-project_user_permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"project_user_permission\",\n  \"type\": \"object\",\n  \"description\": \"A user's direct permission for a given project.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    },\n    \"permission\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-user-project_user_permission-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: project_user_permission
---
