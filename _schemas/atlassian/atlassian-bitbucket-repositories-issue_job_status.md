---
description: The status of an import or export job
layout: schema
name: issue_job_status
properties_list:
- description: ''
  name: type
  type: string
- description: The status of the import/export job
  name: status
  type: string
- description: The phase of the import/export job
  name: phase
  type: string
- description: The total number of issues being imported/exported
  name: total
  type: integer
- description: The total number of issues already imported/exported
  name: count
  type: integer
- description: The percentage of issues already imported/exported
  name: pct
  type: number
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-issue_job_status-schema.json
slug: atlassian-bitbucket-repositories-issue_job_status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"issue_job_status\",\n  \"type\": \"object\",\n  \"description\": \"The status of an import or export job\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the import/export job\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n      \"description\": \"The phase of the import/export job\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of issues being imported/exported\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of issues already imported/exported\"\n    },\n    \"pct\": {\n      \"type\": \"number\",\n      \"description\": \"The percentage of issues already imported/exported\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-issue_job_status-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: issue_job_status
---
