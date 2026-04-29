---
description: ''
layout: schema
name: BenefitPlan
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: name
  type: string
- description: The type of benefit plan (e.g., Medical, Dental, Vision, Life Insurance, 401k).
  name: benefitPlanType
  type: string
- description: ''
  name: isActive
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/benefits-benefit-plan-schema.json
slug: benefits-benefit-plan
source_filename: benefits-benefit-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BenefitPlan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"benefitPlanType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of benefit plan (e.g., Medical, Dental, Vision, Life Insurance, 401k).\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/benefits-benefit-plan-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: BenefitPlan
---
