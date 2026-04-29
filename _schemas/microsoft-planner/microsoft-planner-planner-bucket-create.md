---
description: Request body for creating a new bucket
layout: schema
name: PlannerBucketCreate
properties_list:
- description: Name of the bucket
  name: name
  type: string
- description: ID of the plan the bucket belongs to
  name: planId
  type: string
- description: Hint used to order the bucket
  name: orderHint
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-bucket-create-schema.json
slug: microsoft-planner-planner-bucket-create
source_filename: microsoft-planner-planner-bucket-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerBucketCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new bucket\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the bucket\"\n    },\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the plan the bucket belongs to\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order the bucket\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-bucket-create-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerBucketCreate
---
