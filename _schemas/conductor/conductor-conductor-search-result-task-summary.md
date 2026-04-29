---
description: ''
layout: schema
name: SearchResultTaskSummary
properties_list:
- description: Total number of matching results
  name: totalHits
  type: integer
- description: List of task summaries
  name: results
  type: array
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-search-result-task-summary-schema.json
slug: conductor-conductor-search-result-task-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResultTaskSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalHits\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching results\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of task summaries\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-search-result-task-summary-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: SearchResultTaskSummary
---
