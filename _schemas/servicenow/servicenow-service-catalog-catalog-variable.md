---
description: A variable on a catalog item form.
layout: schema
name: CatalogVariable
properties_list:
- description: The internal name of the variable.
  name: name
  type: string
- description: The display label.
  name: label
  type: string
- description: The variable type.
  name: type
  type: string
- description: Whether the variable is required.
  name: mandatory
  type: boolean
- description: The default value.
  name: default_value
  type: string
- description: Available choices for select-type variables.
  name: choices
  type: array
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-catalog-variable-schema.json
slug: servicenow-service-catalog-catalog-variable
source_filename: servicenow-service-catalog-catalog-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A variable on a catalog item form.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The internal name of the variable.\",\n      \"example\": \"Example Title\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display label.\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The variable type.\",\n      \"example\": \"example_value\"\n    },\n    \"mandatory\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the variable is required.\",\n      \"example\": true\n    },\n    \"default_value\": {\n      \"type\": \"string\",\n      \"description\": \"The default value.\",\n      \"example\": \"example_value\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"Available choices for select-type variables.\",\n      \"example\": [],\n\
  \      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogVariable\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-catalog-variable-schema.json
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
title: CatalogVariable
---
