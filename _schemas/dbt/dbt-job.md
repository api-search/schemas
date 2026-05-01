---
description: A dbt Cloud job that executes a sequence of dbt commands on a schedule or trigger.
layout: schema
name: dbt Cloud Job
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
  name: environment_id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: execute_steps
  type: array
- description: ''
  name: dbt_version
  type: string
- description: ''
  name: triggers
  type: object
- description: ''
  name: schedule
  type: object
- description: ''
  name: state
  type: integer
- description: ''
  name: generate_docs
  type: boolean
- description: ''
  name: run_generate_sources
  type: boolean
provider_name: dbt
provider_slug: dbt
schema_file: json-schema/dbt-job.json
slug: dbt-job
source_filename: dbt-job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/dbt/json-schema/dbt-job.json\",\n  \"title\": \"dbt Cloud Job\",\n  \"description\": \"A dbt Cloud job that executes a sequence of dbt commands on a schedule or trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"integer\"},\n    \"account_id\": {\"type\": \"integer\"},\n    \"project_id\": {\"type\": \"integer\"},\n    \"environment_id\": {\"type\": \"integer\"},\n    \"name\": {\"type\": \"string\"},\n    \"execute_steps\": {\"type\": \"array\", \"items\": {\"type\": \"string\"}},\n    \"dbt_version\": {\"type\": \"string\"},\n    \"triggers\": {\"type\": \"object\"},\n    \"schedule\": {\"type\": \"object\"},\n    \"state\": {\"type\": \"integer\"},\n    \"generate_docs\": {\"type\": \"boolean\"},\n    \"run_generate_sources\": {\"type\": \"boolean\"}\n  },\n  \"required\": [\"id\", \"account_id\", \"project_id\", \"name\"]\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dbt/refs/heads/main/json-schema/dbt-job.json
tags:
- Analytics Engineering
- Data
- ELT
- Metrics
- Projects
- SQL
- Transformation
title: dbt Cloud Job
---
