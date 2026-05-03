---
description: Represents a payroll input entry in the Workday Payroll system, used for additional pay components, deductions, or adjustments to be processed in a payroll run.
layout: schema
name: Payroll Input
properties_list:
- description: The unique Workday identifier for the payroll input
  name: id
  type: string
- description: The display name of the payroll input
  name: descriptor
  type: string
- description: The worker this payroll input applies to
  name: worker
  type: object
- description: The pay component (earnings, deduction, or contribution type)
  name: payComponent
  type: object
- description: The monetary amount for the payroll input
  name: amount
  type: number
- description: The currency of the amount
  name: currency
  type: object
- description: The start date for the payroll input
  name: startDate
  type: string
- description: The end date for the payroll input
  name: endDate
  type:
  - string
  - 'null'
- description: The pay group for processing
  name: payGroup
  type: object
- description: The position associated with the payroll input
  name: position
  type: object
- description: Worktags for financial categorization
  name: worktags
  type: array
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-payroll-schema.json
slug: workday-integration-payroll
source_filename: workday-integration-payroll-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/payrollInput\",\n  \"title\": \"Payroll Input\",\n  \"description\": \"Represents a payroll input entry in the Workday Payroll system, used for additional pay components, deductions, or adjustments to be processed in a payroll run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the payroll input\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the payroll input\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker this payroll input applies to\"\n    },\n    \"payComponent\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay component (earnings, deduction, or contribution type)\"\n    },\n    \"amount\": {\n   \
  \   \"type\": \"number\",\n      \"description\": \"The monetary amount for the payroll input\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The currency of the amount\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The start date for the payroll input\"\n    },\n    \"endDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The end date for the payroll input\"\n    },\n    \"payGroup\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay group for processing\"\n    },\n    \"position\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The position associated with the payroll input\"\n    },\n    \"worktags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ResourceReference\"\n      },\n      \"description\": \"Worktags for\
  \ financial categorization\"\n    }\n  },\n  \"required\": [\"id\", \"worker\", \"payComponent\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-payroll-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Payroll Input
---
