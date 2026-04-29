---
description: A catalog item summary.
layout: schema
name: CatalogItem
properties_list:
- description: Unique identifier for the catalog item.
  name: sys_id
  type: string
- description: The display name of the item.
  name: name
  type: string
- description: A brief description of the item.
  name: short_description
  type: string
- description: The category sys_id.
  name: category
  type: string
- description: The displayed price of the item.
  name: price
  type: string
- description: URL to the item picture.
  name: picture
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-catalog-item-schema.json
slug: servicenow-service-catalog-catalog-item
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A catalog item summary.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the catalog item.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the item.\",\n      \"example\": \"Example Title\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the item.\",\n      \"example\": \"example_value\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category sys_id.\",\n      \"example\": \"example_value\"\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\": \"The displayed price of the item.\",\n      \"example\": \"example_value\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the item picture.\",\n      \"example\"\
  : \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-catalog-item-schema.json
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
title: CatalogItem
---
