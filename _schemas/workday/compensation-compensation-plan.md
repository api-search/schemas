---
description: ''
layout: schema
name: CompensationPlan
properties_list:
- description: The Workday ID of the compensation plan.
  name: id
  type: string
- description: A display descriptor for the plan.
  name: descriptor
  type: string
- description: The type of compensation plan (e.g., Salary, Allowance, Bonus).
  name: compensationPlanType
  type: string
- description: The compensation amount.
  name: amount
  type: number
- description: ''
  name: effectiveDate
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation-compensation-plan-schema.json
slug: compensation-compensation-plan
source_filename: compensation-compensation-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompensationPlan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the compensation plan.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the plan.\"\n    },\n    \"compensationPlanType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of compensation plan (e.g., Salary, Allowance, Bonus).\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The compensation amount.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation-compensation-plan-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: CompensationPlan
---
