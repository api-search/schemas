---
description: The metadata that describes a pull request merge.
layout: schema
name: pullrequest_merge_parameters
properties_list:
- description: ''
  name: type
  type: string
- description: The commit message that will be used on the resulting commit.
  name: message
  type: string
- description: Whether the source branch should be deleted. If this is not provided, we fallback to the value used when the pull request was created, which defaults to False
  name: close_source_branch
  type: boolean
- description: The merge strategy that will be used to merge the pull request.
  name: merge_strategy
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-pullrequest_merge_parameters-schema.json
slug: atlassian-bitbucket-repositories-pullrequest_merge_parameters
source_filename: atlassian-bitbucket-repositories-pullrequest_merge_parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"pullrequest_merge_parameters\",\n  \"type\": \"object\",\n  \"description\": \"The metadata that describes a pull request merge.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The commit message that will be used on the resulting commit.\"\n    },\n    \"close_source_branch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the source branch should be deleted. If this is not provided, we fallback to the value used when the pull request was created, which defaults to False\"\n    },\n    \"merge_strategy\": {\n      \"type\": \"string\",\n      \"description\": \"The merge strategy that will be used to merge the pull request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-pullrequest_merge_parameters-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: pullrequest_merge_parameters
---
