---
description: The result of a submitted catalog order.
layout: schema
name: OrderResult
properties_list:
- description: The generated request number.
  name: request_number
  type: string
- description: The sys_id of the request record.
  name: request_id
  type: string
- description: The table name where the request is stored.
  name: table
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-order-result-schema.json
slug: servicenow-service-catalog-order-result
source_filename: servicenow-service-catalog-order-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a submitted catalog order.\",\n  \"properties\": {\n    \"request_number\": {\n      \"type\": \"string\",\n      \"description\": \"The generated request number.\",\n      \"example\": \"example_value\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the request record.\",\n      \"example\": \"500123\"\n    },\n    \"table\": {\n      \"type\": \"string\",\n      \"description\": \"The table name where the request is stored.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-order-result-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: OrderResult
---
