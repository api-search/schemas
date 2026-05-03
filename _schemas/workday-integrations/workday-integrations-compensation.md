---
description: Represents compensation details for a worker in Workday, including base pay, compensation plans, grades, and total annualized compensation amounts.
layout: schema
name: Workday Compensation Detail
properties_list:
- description: ''
  name: worker
  type: object
- description: Effective date of the compensation plan
  name: effectiveDate
  type: string
- description: Total annualized base pay amount
  name: totalBasePayAnnualized
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Individual compensation plan assignments
  name: compensationPlans
  type: array
- description: ''
  name: compensationGrade
  type: object
- description: ''
  name: compensationStep
  type: object
provider_name: Workday Integrations
provider_slug: workday-integrations
schema_file: json-schema/workday-integrations-compensation-schema.json
slug: workday-integrations-compensation
source_filename: workday-integrations-compensation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-integrations/compensation.json\",\n  \"title\": \"Workday Compensation Detail\",\n  \"description\": \"Represents compensation details for a worker in Workday, including base pay, compensation plans, grades, and total annualized compensation amounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"worker\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Effective date of the compensation plan\"\n    },\n    \"totalBasePayAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Total annualized base pay amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"compensationPlans\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Individual compensation plan assignments\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CompensationPlanAssignment\"\n      }\n    },\n    \"compensationGrade\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"compensationStep\": {\n      \"$ref\": \"#/$defs/Reference\"\n    }\n  },\n  \"$defs\": {\n    \"CompensationPlanAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"A specific compensation plan assigned to a worker\",\n      \"properties\": {\n        \"compensationPlan\": {\n          \"$ref\": \"#/$defs/Reference\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Compensation amount\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        },\n        \"frequency\": {\n          \"type\": \"string\",\n          \"enum\": [\"Annual\", \"Monthly\", \"Hourly\"\
  ],\n          \"description\": \"Payment frequency\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Workday business object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID of the referenced object\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the referenced object\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the referenced resource\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/json-schema/workday-integrations-compensation-schema.json
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
title: Workday Compensation Detail
---
