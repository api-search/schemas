---
description: Represents compensation data for a worker in Workday, including salary plans, allowance plans, bonus plans, and total compensation details.
layout: schema
name: Compensation
properties_list:
- description: The Workday ID of the compensation record.
  name: id
  type: string
- description: A display descriptor for the compensation record.
  name: descriptor
  type: string
- description: The worker this compensation belongs to.
  name: worker
  type: object
- description: The effective date of the compensation.
  name: effectiveDate
  type: string
- description: The compensation plans assigned to the worker.
  name: compensationPlans
  type: array
- description: The total base pay amount across all salary plans.
  name: totalBasePayAmount
  type: number
- description: The annualized total base pay amount.
  name: totalBasePayAnnualizedAmount
  type: number
- description: Total salary and allowances combined.
  name: totalSalaryAndAllowancesAmount
  type: number
- description: The primary compensation basis amount.
  name: primaryCompensationBasis
  type: number
- description: The currency for compensation amounts.
  name: currency
  type: object
- description: The pay frequency (e.g., Annual, Monthly, Bi-Weekly, Weekly).
  name: frequency
  type: object
- description: The compensation grade.
  name: compensationGrade
  type: object
- description: The compensation grade profile.
  name: compensationGradeProfile
  type: object
- description: The compensation step within the grade.
  name: compensationStep
  type: object
- description: The compa-ratio (current pay relative to midpoint of compensation range).
  name: compaRatio
  type: number
- description: The range position (where in the pay range the worker falls).
  name: rangePosition
  type: number
- description: The pay rate type (e.g., Salary, Hourly).
  name: payRateType
  type: object
- description: A link to the full compensation resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/compensation.json
slug: compensation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://workday.com/schemas/compensation.json\",\n  \"title\": \"Compensation\",\n  \"description\": \"Represents compensation data for a worker in Workday, including salary plans, allowance plans, bonus plans, and total compensation details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the compensation record.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the compensation record.\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker this compensation belongs to.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The effective date of the compensation.\"\n    },\n    \"compensationPlans\": {\n      \"type\": \"\
  array\",\n      \"description\": \"The compensation plans assigned to the worker.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CompensationPlan\"\n      }\n    },\n    \"totalBasePayAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The total base pay amount across all salary plans.\"\n    },\n    \"totalBasePayAnnualizedAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The annualized total base pay amount.\"\n    },\n    \"totalSalaryAndAllowancesAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total salary and allowances combined.\"\n    },\n    \"primaryCompensationBasis\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The primary compensation basis amount.\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The currency for compensation amounts.\"\
  \n    },\n    \"frequency\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay frequency (e.g., Annual, Monthly, Bi-Weekly, Weekly).\"\n    },\n    \"compensationGrade\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The compensation grade.\"\n    },\n    \"compensationGradeProfile\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The compensation grade profile.\"\n    },\n    \"compensationStep\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The compensation step within the grade.\"\n    },\n    \"compaRatio\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The compa-ratio (current pay relative to midpoint of compensation range).\"\n    },\n    \"rangePosition\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The range position (where in the pay range the worker falls).\"\n    },\n\
  \    \"payRateType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay rate type (e.g., Salary, Hourly).\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A link to the full compensation resource.\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"CompensationPlan\": {\n      \"type\": \"object\",\n      \"description\": \"A specific compensation plan assigned to a worker.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the compensation plan assignment.\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"A display descriptor for the plan.\"\n        },\n        \"compensationPlanType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of plan (e.g., Salary, Allowance, Bonus, Commission, Stock).\",\n          \"enum\": [\"Salary\"\
  , \"Allowance\", \"Bonus\", \"Commission\", \"Stock\", \"Merit\", \"One-Time Payment\"]\n        },\n        \"compensationPlan\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The compensation plan definition.\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"The compensation amount.\"\n        },\n        \"percentage\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"The compensation percentage (for percentage-based plans).\"\n        },\n        \"currency\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The currency of the amount.\"\n        },\n        \"frequency\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The pay frequency for this plan.\"\n        },\n        \"effectiveDate\": {\n          \"type\": \"string\",\n          \"\
  format\": \"date\",\n          \"description\": \"The effective date of the plan assignment.\"\n        },\n        \"compensationGrade\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        },\n        \"compensationStep\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        }\n      }\n    },\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the referenced resource.\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"A display descriptor for the referenced resource.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A link to the referenced resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/compensation.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Compensation
---
