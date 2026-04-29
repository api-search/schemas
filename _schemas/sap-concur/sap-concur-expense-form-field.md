---
description: A configured form field with its metadata, display properties, and validation rules.
layout: schema
name: FormField
properties_list:
- description: The field identifier
  name: id
  type: string
- description: The localized display label
  name: label
  type: string
- description: The UI control type for rendering
  name: controlType
  type: string
- description: The data type of the field value
  name: dataType
  type: string
- description: Whether the field is mandatory
  name: isRequired
  type: boolean
- description: Whether this is a customer-configured custom field
  name: isCustom
  type: boolean
- description: Maximum allowed character length
  name: maxLength
  type: integer
- description: Display order sequence number
  name: sequence
  type: integer
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-form-field-schema.json
slug: sap-concur-expense-form-field
source_filename: sap-concur-expense-form-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FormField\",\n  \"type\": \"object\",\n  \"description\": \"A configured form field with its metadata, display properties, and validation rules.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The field identifier\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The localized display label\"\n    },\n    \"controlType\": {\n      \"type\": \"string\",\n      \"description\": \"The UI control type for rendering\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the field value\"\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the field is mandatory\"\n    },\n    \"isCustom\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a customer-configured custom field\"\n    },\n    \"maxLength\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Maximum allowed character length\"\n    },\n    \"sequence\": {\n      \"type\": \"integer\",\n      \"description\": \"Display order sequence number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-form-field-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: FormField
---
