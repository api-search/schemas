---
description: A file object, representing a file at a commit in a repository
layout: schema
name: commit_file
properties_list:
- description: ''
  name: type
  type: string
- description: The path in the repository
  name: path
  type: string
- description: ''
  name: attributes
  type: string
- description: The escaped version of the path as it appears in a diff. If the path does not require escaping this will be the same as path.
  name: escaped_path
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-workspaces-commit_file-schema.json
slug: atlassian-bitbucket-workspaces-commit_file
source_filename: atlassian-bitbucket-workspaces-commit_file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"commit_file\",\n  \"type\": \"object\",\n  \"description\": \"A file object, representing a file at a commit in a repository\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path in the repository\"\n    },\n    \"attributes\": {\n      \"type\": \"string\"\n    },\n    \"escaped_path\": {\n      \"type\": \"string\",\n      \"description\": \"The escaped version of the path as it appears in a diff. If the path does not require escaping this will be the same as path.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-workspaces-commit_file-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: commit_file
---
