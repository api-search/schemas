---
description: A pay run represents a single payroll processing cycle for a pay group, encompassing the calculation, review, and completion of payroll for a specific pay period.
layout: schema
name: Workday Payroll Pay Run
properties_list:
- description: Unique identifier for the pay run
  name: id
  type: string
- description: Human-readable name of the pay run
  name: descriptor
  type: string
- description: ''
  name: payGroup
  type: object
- description: ''
  name: payPeriod
  type: object
- description: Current status of the pay run
  name: status
  type: string
- description: Category of the pay run indicating whether it is a regular, off-cycle, or on-demand run
  name: runCategory
  type: string
- description: Date payments will be distributed to workers
  name: paymentDate
  type: string
- description: Total gross pay for all workers in the pay run
  name: totalGrossPay
  type: number
- description: Total net pay after deductions and taxes
  name: totalNetPay
  type: number
- description: Total deductions across all workers
  name: totalDeductions
  type: number
- description: Total tax withholdings across all workers
  name: totalTaxes
  type: number
- description: Number of workers included in the pay run
  name: workerCount
  type: integer
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Timestamp when the pay run was created
  name: createdOn
  type: string
- description: Timestamp when the pay run was completed
  name: completedOn
  type:
  - string
  - 'null'
provider_name: Workday Payroll
provider_slug: workday-payroll
schema_file: json-schema/workday-payroll-pay-run-schema.json
slug: workday-payroll-pay-run
source_filename: workday-payroll-pay-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-payroll/pay-run.json\",\n  \"title\": \"Workday Payroll Pay Run\",\n  \"description\": \"A pay run represents a single payroll processing cycle for a pay group, encompassing the calculation, review, and completion of payroll for a specific pay period.\",\n  \"type\": \"object\",\n  \"required\": [\"payGroup\", \"payPeriod\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the pay run\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the pay run\"\n    },\n    \"payGroup\": {\n      \"$ref\": \"#/$defs/PayGroupRef\"\n    },\n    \"payPeriod\": {\n      \"$ref\": \"#/$defs/PayPeriod\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"InProgress\", \"Completed\", \"Cancelled\"],\n\
  \      \"description\": \"Current status of the pay run\"\n    },\n    \"runCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"Regular\", \"OffCycle\", \"OnDemand\"],\n      \"description\": \"Category of the pay run indicating whether it is a regular, off-cycle, or on-demand run\"\n    },\n    \"paymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date payments will be distributed to workers\"\n    },\n    \"totalGrossPay\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total gross pay for all workers in the pay run\"\n    },\n    \"totalNetPay\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total net pay after deductions and taxes\"\n    },\n    \"totalDeductions\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total deductions across all workers\"\n    },\n    \"totalTaxes\": {\n      \"type\": \"number\",\n      \"minimum\"\
  : 0,\n      \"description\": \"Total tax withholdings across all workers\"\n    },\n    \"workerCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of workers included in the pay run\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the pay run was created\"\n    },\n    \"completedOn\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the pay run was completed\"\n    }\n  },\n  \"$defs\": {\n    \"PayGroupRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a pay group that organizes workers for payroll processing\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Pay group unique identifier\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Pay group display name\"\n        }\n      }\n    },\n    \"PayPeriod\": {\n      \"type\": \"object\",\n      \"description\": \"Date range defining the pay period covered by the run\",\n      \"required\": [\"startDate\", \"endDate\"],\n      \"properties\": {\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Start date of the pay period\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"End date of the pay period\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/json-schema/workday-payroll-pay-run-schema.json
tags:
- Compensation
- Enterprise
- Human-Resources
- Payroll
- Saas
- Tax
title: Workday Payroll Pay Run
---
