---
description: An integration workflow in the Apifuse platform.
layout: schema
name: Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: string
- description: Name of the workflow.
  name: name
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: Type of trigger that activates the workflow.
  name: triggerType
  type: string
provider_name: Apifuse
provider_slug: apifuse
schema_file: json-schema/apifuse-workflow-schema.json
slug: apifuse-workflow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-workflow-schema.json\",\n  \"title\": \"Workflow\",\n  \"description\": \"An integration workflow in the Apifuse platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the workflow.\",\n      \"example\": \"wf-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow.\",\n      \"example\": \"Lead Sync\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"draft\"\n      ],\n      \"description\": \"Current status of the workflow.\"\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"polling\",\n        \"realtime\",\n        \"scheduled\",\n    \
  \    \"webhook\"\n      ],\n      \"description\": \"Type of trigger that activates the workflow.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-workflow-schema.json
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
title: Workflow
---
