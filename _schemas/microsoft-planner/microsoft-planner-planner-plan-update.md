---
description: Request body for updating a plan
layout: schema
name: PlannerPlanUpdate
properties_list:
- description: Updated title of the plan
  name: title
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-plan-update-schema.json
slug: microsoft-planner-planner-plan-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerPlanUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a plan\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Updated title of the plan\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-plan-update-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerPlanUpdate
---
