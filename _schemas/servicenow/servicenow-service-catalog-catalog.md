---
description: A ServiceNow service catalog.
layout: schema
name: Catalog
properties_list:
- description: Unique identifier for the catalog.
  name: sys_id
  type: string
- description: The display title of the catalog.
  name: title
  type: string
- description: A description of the catalog.
  name: description
  type: string
- description: Whether the catalog has categories.
  name: has_categories
  type: boolean
- description: Whether the catalog has items.
  name: has_items
  type: boolean
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-catalog-schema.json
slug: servicenow-service-catalog-catalog
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A ServiceNow service catalog.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the catalog.\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the catalog.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the catalog.\",\n      \"example\": \"A sample description.\"\n    },\n    \"has_categories\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the catalog has categories.\",\n      \"example\": true\n    },\n    \"has_items\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the catalog has items.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Catalog\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-catalog-schema.json
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
title: Catalog
---
