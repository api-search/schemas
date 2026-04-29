---
description: Represents a plan in Microsoft 365. A plan is owned by a group and contains a collection of plannerTasks. It can also have a collection of plannerBuckets.
layout: schema
name: PlannerPlan
properties_list:
- description: The ETag of the resource, used for concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier for the plan. 28 characters long and case-sensitive.
  name: id
  type: string
- description: Title of the plan
  name: title
  type: string
- description: Deprecated. Use the container property instead. ID of the group that owns the plan.
  name: owner
  type: string
- description: The date and time at which the plan was created. ISO 8601 format, always in UTC.
  name: createdDateTime
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-plan-schema.json
slug: microsoft-planner-planner-plan
source_filename: microsoft-planner-planner-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerPlan\",\n  \"type\": \"object\",\n  \"description\": \"Represents a plan in Microsoft 365. A plan is owned by a group and contains a collection of plannerTasks. It can also have a collection of plannerBuckets.\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource, used for concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the plan. 28 characters long and case-sensitive.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the plan\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Deprecated. Use the container property instead. ID of the group that owns the plan.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and\
  \ time at which the plan was created. ISO 8601 format, always in UTC.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-plan-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerPlan
---
