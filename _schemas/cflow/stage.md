---
description: A Stage represents a step in a workflow process where requests are reviewed, approved, or routed.
layout: schema
name: Cflow Stage
properties_list:
- description: Unique identifier of the stage.
  name: id
  type: string
- description: Name of the process stage.
  name: name
  type: string
- description: Order of the stage in the workflow.
  name: order
  type: integer
- description: Users assigned as reviewers for this stage.
  name: reviewers
  type: array
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/stage.json
slug: stage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cflow/blob/main/json-schema/stage.json\",\n  \"title\": \"Cflow Stage\",\n  \"description\": \"A Stage represents a step in a workflow process where requests are reviewed, approved, or routed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the stage.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the process stage.\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Order of the stage in the workflow.\"\n    },\n    \"reviewers\": {\n      \"type\": \"array\",\n      \"description\": \"Users assigned as reviewers for this stage.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/json-schema/stage.json
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Stage
---
