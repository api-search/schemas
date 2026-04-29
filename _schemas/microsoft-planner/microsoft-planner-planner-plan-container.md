---
description: Represents the container for a plannerPlan. The container is a resource that specifies authorization rules and the lifecycle of the plan.
layout: schema
name: PlannerPlanContainer
properties_list:
- description: The identifier of the resource that contains the plan
  name: containerId
  type: string
- description: The type of the container
  name: type
  type: string
- description: The full canonical URL of the container
  name: url
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-plan-container-schema.json
slug: microsoft-planner-planner-plan-container
source_filename: microsoft-planner-planner-plan-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerPlanContainer\",\n  \"type\": \"object\",\n  \"description\": \"Represents the container for a plannerPlan. The container is a resource that specifies authorization rules and the lifecycle of the plan.\",\n  \"properties\": {\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the resource that contains the plan\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the container\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The full canonical URL of the container\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-plan-container-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerPlanContainer
---
