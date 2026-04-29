---
description: Error response from the API
layout: schema
name: Error
properties_list:
- description: ''
  name: Fault
  type: object
- description: ''
  name: time
  type: string
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-error-schema.json
slug: quickbooks-accounting-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Error response from the API\",\n  \"properties\": {\n    \"Fault\": {\n      \"type\": \"object\"\n    },\n    \"time\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-error-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: Error
---
