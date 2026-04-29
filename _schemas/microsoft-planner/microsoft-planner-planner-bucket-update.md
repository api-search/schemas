---
description: Request body for updating a bucket
layout: schema
name: PlannerBucketUpdate
properties_list:
- description: Updated name of the bucket
  name: name
  type: string
- description: Updated order hint for the bucket
  name: orderHint
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-bucket-update-schema.json
slug: microsoft-planner-planner-bucket-update
source_filename: microsoft-planner-planner-bucket-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerBucketUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a bucket\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Updated name of the bucket\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Updated order hint for the bucket\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-bucket-update-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerBucketUpdate
---
