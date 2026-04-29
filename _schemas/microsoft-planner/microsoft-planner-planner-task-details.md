---
description: Represents the additional information about a task, including description, checklist items, and external references.
layout: schema
name: PlannerTaskDetails
properties_list:
- description: The ETag of the resource
  name: '@odata.etag'
  type: string
- description: The unique identifier for the task details
  name: id
  type: string
- description: Description of the task
  name: description
  type: string
- description: The type of preview shown on the task
  name: previewType
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-task-details-schema.json
slug: microsoft-planner-planner-task-details
source_filename: microsoft-planner-planner-task-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerTaskDetails\",\n  \"type\": \"object\",\n  \"description\": \"Represents the additional information about a task, including description, checklist items, and external references.\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the task details\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the task\"\n    },\n    \"previewType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of preview shown on the task\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-task-details-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerTaskDetails
---
