---
description: SOAP envelope containing a signal event to post to a workflow, including the workflow ID, signal activity name, and optional XML variables.
layout: schema
name: WorkflowPostEventRequest
properties_list:
- description: Internal ID of the target workflow.
  name: workflowId
  type: integer
- description: Name of the external signal activity in the workflow.
  name: activity
  type: string
- description: XML element containing variable parameters to pass to the workflow transition.
  name: variables
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-workflow-post-event-request-schema.json
slug: adobe-campaign-classic-workflow-post-event-request
source_filename: adobe-campaign-classic-workflow-post-event-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-workflow-post-event-request-schema.json\",\n  \"title\": \"WorkflowPostEventRequest\",\n  \"description\": \"SOAP envelope containing a signal event to post to a workflow, including the workflow ID, signal activity name, and optional XML variables.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal ID of the target workflow.\",\n      \"example\": 42\n    },\n    \"activity\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the external signal activity in the workflow.\",\n      \"example\": \"example_value\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"XML element containing variable parameters to pass to the workflow transition.\",\n    \
  \  \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-workflow-post-event-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WorkflowPostEventRequest
---
