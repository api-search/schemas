---
description: Human-readable labels for the action
layout: schema
name: ActionLabels
properties_list:
- description: The display name of the action
  name: actionName
  type: string
- description: A description of what the action does
  name: actionDescription
  type: string
- description: The name of the app providing this action
  name: appDisplayName
  type: string
- description: Content to display on the action card in the workflow editor
  name: actionCardContent
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-action-labels-schema.json
slug: hubspot-custom-workflow-actions-action-labels
source_filename: hubspot-custom-workflow-actions-action-labels-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Human-readable labels for the action\",\n  \"properties\": {\n    \"actionName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the action\",\n      \"example\": \"Example Record\"\n    },\n    \"actionDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the action does\",\n      \"example\": \"This is an example description.\"\n    },\n    \"appDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the app providing this action\",\n      \"example\": \"Example Record\"\n    },\n    \"actionCardContent\": {\n      \"type\": \"string\",\n      \"description\": \"Content to display on the action card in the workflow editor\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"actionName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionLabels\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-action-labels-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ActionLabels
---
