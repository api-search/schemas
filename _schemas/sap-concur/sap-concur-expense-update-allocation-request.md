---
description: Request body for updating an allocation
layout: schema
name: UpdateAllocationRequest
properties_list:
- description: The allocation fields to update
  name: allocation
  type: object
- description: The expense IDs to which this update applies
  name: expenseIds
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-update-allocation-request-schema.json
slug: sap-concur-expense-update-allocation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateAllocationRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an allocation\",\n  \"properties\": {\n    \"allocation\": {\n      \"type\": \"object\",\n      \"description\": \"The allocation fields to update\"\n    },\n    \"expenseIds\": {\n      \"type\": \"array\",\n      \"description\": \"The expense IDs to which this update applies\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-update-allocation-request-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: UpdateAllocationRequest
---
