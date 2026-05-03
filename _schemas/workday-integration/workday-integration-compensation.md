---
description: Represents compensation data for a worker within the Workday system, including base pay, bonuses, and equity.
layout: schema
name: Compensation
properties_list:
- description: The unique Workday identifier for the compensation record
  name: id
  type: string
- description: The display name of the compensation record
  name: descriptor
  type: string
- description: The worker this compensation is associated with
  name: worker
  type: object
- description: The compensation plan
  name: compensationPlan
  type: object
- description: The compensation amount
  name: amount
  type: number
- description: The currency of the compensation
  name: currency
  type: object
- description: The payment frequency (Annual, Monthly, Hourly)
  name: frequency
  type: object
- description: The date the compensation became effective
  name: effectiveDate
  type: string
- description: The pay grade associated with the compensation
  name: payGrade
  type: object
- description: The pay step within the pay grade
  name: payStep
  type: object
- description: The total base pay amount
  name: totalBasePay
  type: number
- description: The total salary including all allowances
  name: totalSalaryAndAllowances
  type: number
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-compensation-schema.json
slug: workday-integration-compensation
source_filename: workday-integration-compensation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/compensation\",\n  \"title\": \"Compensation\",\n  \"description\": \"Represents compensation data for a worker within the Workday system, including base pay, bonuses, and equity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the compensation record\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the compensation record\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker this compensation is associated with\"\n    },\n    \"compensationPlan\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The compensation plan\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The compensation amount\"\
  \n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The currency of the compensation\"\n    },\n    \"frequency\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The payment frequency (Annual, Monthly, Hourly)\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the compensation became effective\"\n    },\n    \"payGrade\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay grade associated with the compensation\"\n    },\n    \"payStep\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay step within the pay grade\"\n    },\n    \"totalBasePay\": {\n      \"type\": \"number\",\n      \"description\": \"The total base pay amount\"\n    },\n    \"totalSalaryAndAllowances\": {\n      \"type\": \"number\",\n      \"description\": \"The total salary including all allowances\"\
  \n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-compensation-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Compensation
---
