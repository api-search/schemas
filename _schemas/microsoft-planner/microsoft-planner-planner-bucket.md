---
description: Represents a bucket (custom column) for tasks in a plan in Microsoft 365. It is contained in a plannerPlan and can have a collection of plannerTasks.
layout: schema
name: PlannerBucket
properties_list:
- description: The ETag of the resource, used for concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier for the bucket. 28 characters long and case-sensitive.
  name: id
  type: string
- description: Name of the bucket
  name: name
  type: string
- description: Plan ID to which the bucket belongs
  name: planId
  type: string
- description: Hint used to order buckets in a list view
  name: orderHint
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-bucket-schema.json
slug: microsoft-planner-planner-bucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerBucket\",\n  \"type\": \"object\",\n  \"description\": \"Represents a bucket (custom column) for tasks in a plan in Microsoft 365. It is contained in a plannerPlan and can have a collection of plannerTasks.\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource, used for concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the bucket. 28 characters long and case-sensitive.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the bucket\"\n    },\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"Plan ID to which the bucket belongs\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order buckets in a list view\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-bucket-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerBucket
---
