---
description: Full details of a catalog item including its variables.
layout: schema
name: CatalogItemDetail
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
- description: The full description of the item.
  name: description
  type: string
- description: The category sys_id.
  name: category
  type: string
- description: The displayed price.
  name: price
  type: string
- description: URL to the item picture.
  name: picture
  type: string
- description: Whether a file attachment is required to order the item.
  name: mandatory_attachment
  type: boolean
- description: The method used to fulfill the request.
  name: request_method
  type: string
- description: The list of variables (form fields) that must be filled in when ordering the item.
  name: variables
  type: array
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-service-catalog-catalog-item-detail-schema.json
slug: servicenow-service-catalog-catalog-item-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Full details of a catalog item including its variables.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the catalog item.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the item.\",\n      \"example\": \"Example Title\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the item.\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The full description of the item.\",\n      \"example\": \"A sample description.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category sys_id.\",\n      \"example\": \"example_value\"\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The displayed price.\",\n      \"example\": \"example_value\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the item picture.\",\n      \"example\": \"example_value\"\n    },\n    \"mandatory_attachment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a file attachment is required to order the item.\",\n      \"example\": true\n    },\n    \"request_method\": {\n      \"type\": \"string\",\n      \"description\": \"The method used to fulfill the request.\",\n      \"example\": \"example_value\"\n    },\n    \"variables\": {\n      \"type\": \"array\",\n      \"description\": \"The list of variables (form fields) that must be filled in when ordering the item.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A variable on a catalog item form.\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The\
  \ internal name of the variable.\",\n            \"example\": \"Example Title\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"The display label.\",\n            \"example\": \"Example Title\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The variable type.\",\n            \"example\": \"example_value\"\n          },\n          \"mandatory\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the variable is required.\",\n            \"example\": true\n          },\n          \"default_value\": {\n            \"type\": \"string\",\n            \"description\": \"The default value.\",\n            \"example\": \"example_value\"\n          },\n          \"choices\": {\n            \"type\": \"array\",\n            \"description\": \"Available choices for select-type variables.\",\n            \"example\": [],\n            \"items\": {\n          \
  \    \"type\": \"object\",\n              \"properties\": {\n                \"label\": {\n                  \"type\": \"string\"\n                },\n                \"value\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogItemDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-service-catalog-catalog-item-detail-schema.json
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
title: CatalogItemDetail
---
