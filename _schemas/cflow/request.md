---
description: A Request is a submission within a workflow that moves through stages for review, approval, or rejection.
layout: schema
name: Cflow Request
properties_list:
- description: Unique identifier of the request.
  name: id
  type: string
- description: Identifier of the associated workflow.
  name: workflowId
  type: string
- description: Current status of the request.
  name: status
  type: string
- description: Name or identifier of the current process stage.
  name: currentStage
  type: string
- description: Dynamic key-value pairs representing the form field data for the request.
  name: fields
  type: object
- description: Username of the person who submitted the request.
  name: submittedBy
  type: string
- description: Timestamp when the request was created.
  name: createdAt
  type: string
- description: Timestamp when the request was last updated.
  name: updatedAt
  type: string
provider_name: Cflow
provider_slug: cflow
schema_file: json-schema/request.json
slug: request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cflow/blob/main/json-schema/request.json\",\n  \"title\": \"Cflow Request\",\n  \"description\": \"A Request is a submission within a workflow that moves through stages for review, approval, or rejection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the request.\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the associated workflow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the request.\",\n      \"enum\": [\n        \"draft\",\n        \"pending\",\n        \"approved\",\n        \"rejected\",\n        \"completed\"\n      ]\n    },\n    \"currentStage\": {\n      \"type\": \"string\",\n      \"description\": \"Name or identifier of the current process\
  \ stage.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Dynamic key-value pairs representing the form field data for the request.\",\n      \"additionalProperties\": true\n    },\n    \"submittedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the person who submitted the request.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/json-schema/request.json
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
title: Cflow Request
---
