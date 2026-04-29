---
description: A checklist item on a Planner task
layout: schema
name: PlannerChecklistItem
properties_list:
- description: ''
  name: '@odata.type'
  type: string
- description: Whether the item is checked (completed)
  name: isChecked
  type: boolean
- description: The date and time the item was last modified
  name: lastModifiedDateTime
  type: string
- description: Hint used to order items in the checklist
  name: orderHint
  type: string
- description: Title of the checklist item
  name: title
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-checklist-item-schema.json
slug: microsoft-planner-planner-checklist-item
source_filename: microsoft-planner-planner-checklist-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerChecklistItem\",\n  \"type\": \"object\",\n  \"description\": \"A checklist item on a Planner task\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\"\n    },\n    \"isChecked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the item is checked (completed)\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the item was last modified\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order items in the checklist\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the checklist item\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-checklist-item-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerChecklistItem
---
