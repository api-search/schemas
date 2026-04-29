---
description: ''
layout: schema
name: ProjectUpdateRequest
properties_list:
- description: Updated project name
  name: name
  type: string
- description: Updated project description
  name: description
  type: string
- description: Optional schedule date range for the project
  name: schedule_attributes
  type: object
- description: Controls who can join the project
  name: admissions
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectupdaterequest-schema.json
slug: projectupdaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/projectupdaterequest-schema.json\",\n  \"title\": \"ProjectUpdateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Updated project name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Updated project description\"\n    },\n    \"schedule_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Optional schedule date range for the project\",\n      \"properties\": {\n        \"start_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Project start date in ISO 8601 format\"\n        },\n        \"end_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Project end date\
  \ in ISO 8601 format\"\n        }\n      }\n    },\n    \"admissions\": {\n      \"type\": \"string\",\n      \"description\": \"Controls who can join the project\",\n      \"enum\": [\n        \"invite\",\n        \"employee\",\n        \"team\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/projectupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectUpdateRequest
---
