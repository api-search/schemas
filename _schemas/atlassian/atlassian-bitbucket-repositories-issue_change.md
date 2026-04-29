---
description: An issue change.
layout: schema
name: issue_change
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: links
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: created_on
  type: string
- description: ''
  name: changes
  type: object
- description: ''
  name: message
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-issue_change-schema.json
slug: atlassian-bitbucket-repositories-issue_change
source_filename: atlassian-bitbucket-repositories-issue_change-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"issue_change\",\n  \"type\": \"object\",\n  \"description\": \"An issue change.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\n    },\n    \"changes\": {\n      \"type\": \"object\"\n    },\n    \"message\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-issue_change-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: issue_change
---
