---
description: ''
layout: schema
name: SuccessionPlan
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: Readiness level (e.g., Ready Now, Ready in 1-2 Years).
  name: readiness
  type: string
- description: ''
  name: candidates
  type: array
- description: ''
  name: lastUpdated
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/talent-succession-plan-schema.json
slug: talent-succession-plan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessionPlan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"readiness\": {\n      \"type\": \"string\",\n      \"description\": \"Readiness level (e.g., Ready Now, Ready in 1-2 Years).\"\n    },\n    \"candidates\": {\n      \"type\": \"array\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/talent-succession-plan-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: SuccessionPlan
---
