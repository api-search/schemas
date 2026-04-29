---
description: A catalog category.
layout: schema
name: Category
properties_list:
- description: Unique identifier for the category.
  name: sys_id
  type: string
- description: The display title of the category.
  name: title
  type: string
- description: A description of the category.
  name: description
  type: string
- description: The full description of the category.
  name: full_description
  type: string
- description: Child categories.
  name: subcategories
  type: array
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-category-schema.json
slug: servicenow-service-catalog-category
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A catalog category.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the category.\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the category.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the category.\",\n      \"example\": \"A sample description.\"\n    },\n    \"full_description\": {\n      \"type\": \"string\",\n      \"description\": \"The full description of the category.\",\n      \"example\": \"example_value\"\n    },\n    \"subcategories\": {\n      \"type\": \"array\",\n      \"description\": \"Child categories.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"sys_id\": {\n            \"type\"\
  : \"string\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Category\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-category-schema.json
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
title: Category
---
