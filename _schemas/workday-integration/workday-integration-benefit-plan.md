---
description: Represents a benefit plan enrollment for a worker within the Workday Benefits Administration system.
layout: schema
name: Benefit Plan
properties_list:
- description: The unique Workday identifier for the benefit plan enrollment
  name: id
  type: string
- description: The display name of the benefit plan
  name: descriptor
  type: string
- description: The type of benefit plan (Medical, Dental, Vision, Life, etc.)
  name: planType
  type: object
- description: The date coverage begins
  name: coverageBeginDate
  type: string
- description: The date coverage ends
  name: coverageEndDate
  type:
  - string
  - 'null'
- description: The coverage level (Employee Only, Employee + Spouse, Family, etc.)
  name: coverageLevel
  type: string
- description: The employee contribution cost per period
  name: employeeCost
  type: number
- description: The employer contribution cost per period
  name: employerCost
  type: number
- description: Dependents covered under this plan
  name: dependents
  type: array
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-benefit-plan-schema.json
slug: workday-integration-benefit-plan
source_filename: workday-integration-benefit-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/benefitPlan\",\n  \"title\": \"Benefit Plan\",\n  \"description\": \"Represents a benefit plan enrollment for a worker within the Workday Benefits Administration system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the benefit plan enrollment\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the benefit plan\"\n    },\n    \"planType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of benefit plan (Medical, Dental, Vision, Life, etc.)\"\n    },\n    \"coverageBeginDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date coverage begins\"\n    },\n    \"coverageEndDate\": {\n      \"type\": [\"string\", \"null\"],\n    \
  \  \"format\": \"date\",\n      \"description\": \"The date coverage ends\"\n    },\n    \"coverageLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The coverage level (Employee Only, Employee + Spouse, Family, etc.)\"\n    },\n    \"employeeCost\": {\n      \"type\": \"number\",\n      \"description\": \"The employee contribution cost per period\"\n    },\n    \"employerCost\": {\n      \"type\": \"number\",\n      \"description\": \"The employer contribution cost per period\"\n    },\n    \"dependents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ResourceReference\"\n      },\n      \"description\": \"Dependents covered under this plan\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n   \
  \       \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-benefit-plan-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Benefit Plan
---
