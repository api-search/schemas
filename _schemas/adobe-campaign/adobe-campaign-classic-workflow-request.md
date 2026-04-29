---
description: SOAP envelope containing the workflow internal ID for start/stop operations.
layout: schema
name: WorkflowRequest
properties_list:
- description: Internal ID of the workflow.
  name: workflowId
  type: integer
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-workflow-request-schema.json
slug: adobe-campaign-classic-workflow-request
source_filename: adobe-campaign-classic-workflow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-workflow-request-schema.json\",\n  \"title\": \"WorkflowRequest\",\n  \"description\": \"SOAP envelope containing the workflow internal ID for start/stop operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal ID of the workflow.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-workflow-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: WorkflowRequest
---
