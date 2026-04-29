---
description: A json object representing the repository's inheritance state values
layout: schema
name: repository_inheritance_state
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: override_settings
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-repository_inheritance_state-schema.json
slug: atlassian-bitbucket-repositories-repository_inheritance_state
source_filename: atlassian-bitbucket-repositories-repository_inheritance_state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"repository_inheritance_state\",\n  \"type\": \"object\",\n  \"description\": \"A json object representing the repository's inheritance state values\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"override_settings\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-repository_inheritance_state-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: repository_inheritance_state
---
