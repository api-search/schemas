---
description: A diffstat object that includes a summary of changes made to a file between two commits.
layout: schema
name: diffstat
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: lines_added
  type: integer
- description: ''
  name: lines_removed
  type: integer
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-diffstat-schema.json
slug: atlassian-bitbucket-repositories-diffstat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"diffstat\",\n  \"type\": \"object\",\n  \"description\": \"A diffstat object that includes a summary of changes made to a file between two commits.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lines_added\": {\n      \"type\": \"integer\"\n    },\n    \"lines_removed\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-diffstat-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: diffstat
---
