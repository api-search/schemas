---
description: Custom field defined for the entity
layout: schema
name: CustomField
properties_list:
- description: Unique identifier of the custom field definition
  name: DefinitionId
  type: string
- description: Name of the custom field
  name: Name
  type: string
- description: Data type of the custom field
  name: Type
  type: string
- description: Value when Type is StringType
  name: StringValue
  type: string
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-custom-field-schema.json
slug: quickbooks-accounting-custom-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomField\",\n  \"type\": \"object\",\n  \"description\": \"Custom field defined for the entity\",\n  \"properties\": {\n    \"DefinitionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the custom field definition\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the custom field\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the custom field\"\n    },\n    \"StringValue\": {\n      \"type\": \"string\",\n      \"description\": \"Value when Type is StringType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-custom-field-schema.json
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
title: CustomField
---
