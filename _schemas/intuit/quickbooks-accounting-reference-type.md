---
description: A reference type used throughout the API to link entities. Contains the ID value and optionally the display name of the referenced entity.
layout: schema
name: ReferenceType
properties_list:
- description: The ID of the referenced entity
  name: value
  type: string
- description: An identifying name for the referenced entity
  name: name
  type: string
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-reference-type-schema.json
slug: quickbooks-accounting-reference-type
source_filename: quickbooks-accounting-reference-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReferenceType\",\n  \"type\": \"object\",\n  \"description\": \"A reference type used throughout the API to link entities. Contains the ID value and optionally the display name of the referenced entity.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the referenced entity\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"An identifying name for the referenced entity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-reference-type-schema.json
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
title: ReferenceType
---
