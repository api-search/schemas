---
description: A custom field value configured by the organization. Field IDs follow patterns like custom1-custom40 and orgUnit1-orgUnit6.
layout: schema
name: CustomData
properties_list:
- description: The identifier of the custom field (e.g., custom1, orgUnit1)
  name: id
  type: string
- description: The value assigned to the custom field
  name: value
  type: string
- description: Whether the current value passes validation rules
  name: isValid
  type: boolean
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-custom-data-schema.json
slug: sap-concur-expense-custom-data
source_filename: sap-concur-expense-custom-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomData\",\n  \"type\": \"object\",\n  \"description\": \"A custom field value configured by the organization. Field IDs follow patterns like custom1-custom40 and orgUnit1-orgUnit6.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the custom field (e.g., custom1, orgUnit1)\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value assigned to the custom field\"\n    },\n    \"isValid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current value passes validation rules\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-custom-data-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: CustomData
---
