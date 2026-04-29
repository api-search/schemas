---
description: An expense allocation that distributes an expense amount across cost centers, departments, or general ledger accounts.
layout: schema
name: Allocation
properties_list:
- description: Unique identifier of the allocation
  name: allocationId
  type: string
- description: The expense this allocation belongs to
  name: expenseId
  type: string
- description: The ledger account code
  name: accountCode
  type: string
- description: Account code for amounts exceeding policy limits
  name: overLimitAccountCode
  type: string
- description: The percentage of the total expense allocated (0-100)
  name: percentage
  type: number
- description: Whether this allocation was automatically created by the system (true) or manually created by a user (false)
  name: isSystemAllocation
  type: boolean
- description: Whether the allocation percentage has been modified
  name: isPercentEdited
  type: boolean
- description: Custom field values on the allocation
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-allocation-schema.json
slug: sap-concur-expense-allocation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Allocation\",\n  \"type\": \"object\",\n  \"description\": \"An expense allocation that distributes an expense amount across cost centers, departments, or general ledger accounts.\",\n  \"properties\": {\n    \"allocationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the allocation\"\n    },\n    \"expenseId\": {\n      \"type\": \"string\",\n      \"description\": \"The expense this allocation belongs to\"\n    },\n    \"accountCode\": {\n      \"type\": \"string\",\n      \"description\": \"The ledger account code\"\n    },\n    \"overLimitAccountCode\": {\n      \"type\": \"string\",\n      \"description\": \"Account code for amounts exceeding policy limits\"\n    },\n    \"percentage\": {\n      \"type\": \"number\",\n      \"description\": \"The percentage of the total expense allocated (0-100)\"\n    },\n    \"isSystemAllocation\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether this allocation was automatically created by the system (true) or manually created by a user (false)\"\n    },\n    \"isPercentEdited\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the allocation percentage has been modified\"\n    },\n    \"customData\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field values on the allocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-allocation-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Allocation
---
