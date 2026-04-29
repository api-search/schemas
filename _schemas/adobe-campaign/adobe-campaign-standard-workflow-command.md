---
description: WorkflowCommand from Adobe Campaign API
layout: schema
name: WorkflowCommand
properties_list:
- description: The workflow control command to execute.
  name: method
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-workflow-command-schema.json
slug: adobe-campaign-standard-workflow-command
source_filename: adobe-campaign-standard-workflow-command-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-workflow-command-schema.json\",\n  \"title\": \"WorkflowCommand\",\n  \"description\": \"WorkflowCommand from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"start\",\n        \"pause\",\n        \"resume\",\n        \"stop\"\n      ],\n      \"description\": \"The workflow control command to execute.\",\n      \"example\": \"start\"\n    }\n  },\n  \"required\": [\n    \"method\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-workflow-command-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WorkflowCommand
---
