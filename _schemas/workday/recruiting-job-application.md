---
description: ''
layout: schema
name: JobApplication
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The application status (e.g., In Progress, Offer, Hired, Rejected).
  name: status
  type: string
- description: ''
  name: appliedOn
  type: string
- description: ''
  name: hiredOn
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/recruiting-job-application-schema.json
slug: recruiting-job-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The application status (e.g., In Progress, Offer, Hired, Rejected).\"\n    },\n    \"appliedOn\": {\n      \"type\": \"string\"\n    },\n    \"hiredOn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/recruiting-job-application-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobApplication
---
