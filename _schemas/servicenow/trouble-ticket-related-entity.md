---
description: ''
layout: schema
name: RelatedEntity
properties_list:
- description: This value is always relatedEntity
  name: '@type'
  type: string
- description: Sys_id of the impacted item or service
  name: id
  type: string
- description: Returns an empty string
  name: href
  type: string
- description: Name of the impacted item or service
  name: name
  type: string
- description: Description of the impacted item or service
  name: role
  type: string
- description: Type of item or service
  name: '@referredType'
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-related-entity-schema.json
slug: trouble-ticket-related-entity
source_filename: trouble-ticket-related-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"This value is always relatedEntity\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the impacted item or service\",\n      \"example\": \"abc123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Returns an empty string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the impacted item or service\",\n      \"example\": \"Example Title\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the impacted item or service\",\n      \"example\": \"example_value\"\n    },\n    \"@referredType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of item or service\",\n      \"example\": \"asset\",\n      \"enum\": [\n    \
  \    \"asset\",\n        \"product\",\n        \"product_inventory\",\n        \"cmdb_ci\",\n        \"cmdb_ci_service\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedEntity\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-related-entity-schema.json
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
title: RelatedEntity
---
