---
description: A cost object relevant to an approver, representing how expenses on a report map to organizational cost structures.
layout: schema
name: CostObjectForApprover
properties_list:
- description: Unique identifier of the cost object
  name: costObjectId
  type: string
- description: Display name of the cost object
  name: name
  type: string
- description: Cost object code
  name: code
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-cost-object-for-approver-schema.json
slug: sap-concur-expense-cost-object-for-approver
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CostObjectForApprover\",\n  \"type\": \"object\",\n  \"description\": \"A cost object relevant to an approver, representing how expenses on a report map to organizational cost structures.\",\n  \"properties\": {\n    \"costObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the cost object\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the cost object\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Cost object code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-cost-object-for-approver-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: CostObjectForApprover
---
