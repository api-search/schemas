---
description: A single execution of a dbt Cloud job, including status and timing details.
layout: schema
name: dbt Cloud Run
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: account_id
  type: integer
- description: ''
  name: project_id
  type: integer
- description: ''
  name: job_id
  type: integer
- description: ''
  name: environment_id
  type: integer
- description: Run status (1=queued, 2=starting, 3=running, 10=success, 20=error, 30=cancelled)
  name: status
  type: integer
- description: ''
  name: git_branch
  type: string
- description: ''
  name: git_sha
  type: string
- description: ''
  name: trigger
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: started_at
  type: string
- description: ''
  name: finished_at
  type: string
- description: ''
  name: duration
  type: string
provider_name: dbt
provider_slug: dbt
schema_file: json-schema/dbt-run.json
slug: dbt-run
source_filename: dbt-run.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/dbt/json-schema/dbt-run.json\",\n  \"title\": \"dbt Cloud Run\",\n  \"description\": \"A single execution of a dbt Cloud job, including status and timing details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\"},\n    \"account_id\": {\"type\": \"integer\"},\n    \"project_id\": {\"type\": \"integer\"},\n    \"job_id\": {\"type\": \"integer\"},\n    \"environment_id\": {\"type\": \"integer\"},\n    \"status\": {\"type\": \"integer\", \"description\": \"Run status (1=queued, 2=starting, 3=running, 10=success, 20=error, 30=cancelled)\"},\n    \"git_branch\": {\"type\": \"string\"},\n    \"git_sha\": {\"type\": \"string\"},\n    \"trigger\": {\"type\": \"object\"},\n    \"created_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"started_at\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"finished_at\"\
  : {\"type\": \"string\", \"format\": \"date-time\"},\n    \"duration\": {\"type\": \"string\"}\n  },\n  \"required\": [\"id\", \"job_id\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/json-schema/dbt-run.json
tags:
- Analytics Engineering
- Data
- ELT
- Metrics
- Projects
- SQL
- Transformation
title: dbt Cloud Run
---
