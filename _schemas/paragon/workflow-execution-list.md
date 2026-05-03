---
description: A paginated list of workflow executions returned by the Task History API.
layout: schema
name: Paragon Workflow Execution List
properties_list:
- description: Array of workflow execution records.
  name: data
  type: array
- description: Total number of workflow executions matching the query.
  name: total
  type: integer
- description: URL to retrieve the next page of results. Null if there are no more pages.
  name: nextLink
  type:
  - string
  - 'null'
provider_name: Paragon
provider_slug: paragon
schema_file: json-schema/workflow-execution-list.json
slug: workflow-execution-list
source_filename: workflow-execution-list.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/workflow-execution-list.json\",\n  \"title\": \"Paragon Workflow Execution List\",\n  \"description\": \"A paginated list of workflow executions returned by the Task History API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of workflow execution records.\",\n      \"items\": {\n        \"$ref\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/workflow-execution.json\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of workflow executions matching the query.\"\n    },\n    \"nextLink\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL to retrieve the next page of results. Null if there are no more pages.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/json-schema/workflow-execution-list.json
tags:
- Embedded iPaaS
- Integrations
title: Paragon Workflow Execution List
---
