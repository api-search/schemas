---
description: An executable pipeline command.
layout: schema
name: pipeline_command
properties_list:
- description: The name of the command.
  name: name
  type: string
- description: The executable command.
  name: command
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-pipeline_command-schema.json
slug: atlassian-bitbucket-repositories-pipeline_command
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"pipeline_command\",\n  \"type\": \"object\",\n  \"description\": \"An executable pipeline command.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the command.\"\n    },\n    \"command\": {\n      \"type\": \"string\",\n      \"description\": \"The executable command.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-pipeline_command-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: pipeline_command
---
