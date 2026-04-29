---
description: The resolution object for a Comment.
layout: schema
name: comment_resolution
properties_list:
- description: ''
  name: type
  type: string
- description: The ISO8601 timestamp the resolution was created.
  name: created_on
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-pull-requests-comment_resolution-schema.json
slug: atlassian-bitbucket-pull-requests-comment_resolution
source_filename: atlassian-bitbucket-pull-requests-comment_resolution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"comment_resolution\",\n  \"type\": \"object\",\n  \"description\": \"The resolution object for a Comment.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO8601 timestamp the resolution was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-pull-requests-comment_resolution-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: comment_resolution
---
