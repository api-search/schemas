---
description: A Workflow defines an automated business process with stages, rules, and field configurations in Cflow.
layout: schema
name: Cflow Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: string
- description: Name of the workflow.
  name: name
  type: string
- description: Description of the workflow.
  name: description
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: List of process stages in the workflow.
  name: stages
  type: array
- description: Timestamp when the workflow was created.
  name: createdAt
  type: string
- description: Timestamp when the workflow was last updated.
  name: updatedAt
  type: string
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/workflow.json
slug: workflow
source_filename: workflow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cflow/blob/main/json-schema/workflow.json\",\n  \"title\": \"Cflow Workflow\",\n  \"description\": \"A Workflow defines an automated business process with stages, rules, and field configurations in Cflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workflow.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workflow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the workflow.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"draft\"\n      ]\n    },\n    \"stages\": {\n      \"type\": \"array\",\n      \"description\": \"\
  List of process stages in the workflow.\",\n      \"items\": {\n        \"$ref\": \"stage.json\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workflow was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workflow was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/json-schema/workflow.json
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Workflow
---
