---
description: A ref object, representing a branch or tag in a repository.
layout: schema
name: ref
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: links
  type: object
- description: The name of the ref.
  name: name
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-teams-ref-schema.json
slug: atlassian-bitbucket-teams-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ref\",\n  \"type\": \"object\",\n  \"description\": \"A ref object, representing a branch or tag in a repository.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the ref.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-teams-ref-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ref
---
