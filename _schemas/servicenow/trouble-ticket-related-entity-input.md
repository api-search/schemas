---
description: ''
layout: schema
name: RelatedEntityInput
properties_list:
- description: Sys_id of the impacted item or service
  name: id
  type: string
- description: Type of item or service
  name: '@referredType'
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-related-entity-input-schema.json
slug: trouble-ticket-related-entity-input
source_filename: trouble-ticket-related-entity-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the impacted item or service\",\n      \"example\": \"abc123\"\n    },\n    \"@referredType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of item or service\",\n      \"example\": \"asset\",\n      \"enum\": [\n        \"asset\",\n        \"product\",\n        \"product_inventory\",\n        \"cmdb_ci\",\n        \"cmdb_ci_service\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"@referredType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedEntityInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-related-entity-input-schema.json
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
title: RelatedEntityInput
---
