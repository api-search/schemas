---
description: Request body for creating a new plan
layout: schema
name: PlannerPlanCreate
properties_list:
- description: Title of the plan
  name: title
  type: string
- description: The container for the plan
  name: container
  type: object
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-plan-create-schema.json
slug: microsoft-planner-planner-plan-create
source_filename: microsoft-planner-planner-plan-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerPlanCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new plan\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the plan\"\n    },\n    \"container\": {\n      \"type\": \"object\",\n      \"description\": \"The container for the plan\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-plan-create-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerPlanCreate
---
