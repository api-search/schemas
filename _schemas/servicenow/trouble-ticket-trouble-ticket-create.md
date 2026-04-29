---
description: ''
layout: schema
name: TroubleTicketCreate
properties_list:
- description: Name of the trouble ticket, typically a short description of the issue
  name: name
  type: string
- description: A description of the issue
  name: description
  type: string
- description: 'The severity of the issue (must provide choice value only): - 1: Critical - 2: High - 3: Moderate - 4: Low - 5: Planning (Incident only)'
  name: severity
  type: string
- description: The current status of the trouble ticket (can provide choice label or value)
  name: status
  type: string
- description: The type of ticket to create
  name: ticketType
  type: string
- description: ''
  name: channel
  type: object
- description: List of work notes and comments to add to the ticket
  name: note
  type: array
- description: List of impacted assets, products, sold products, configuration items, or services
  name: relatedEntity
  type: array
- description: Details about contacts for the ticket
  name: relatedParty
  type: array
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-trouble-ticket-create-schema.json
slug: trouble-ticket-trouble-ticket-create
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the trouble ticket, typically a short description of the issue\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the issue\",\n      \"example\": \"A sample description.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity of the issue (must provide choice value only):\\n- 1: Critical\\n- 2: High\\n- 3: Moderate\\n- 4: Low\\n- 5: Planning (Incident only)\\n\",\n      \"example\": \"1\",\n      \"enum\": [\n        \"1\",\n        \"2\",\n        \"3\",\n        \"4\",\n        \"5\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the trouble ticket (can provide choice label or value)\",\n      \"example\": \"example_value\"\n    },\n    \"ticketType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The type of ticket to create\",\n      \"example\": \"Case\",\n      \"enum\": [\n        \"Case\",\n        \"Incident\",\n        \"Service Problem Case\"\n      ]\n    },\n    \"channel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the contact method (can provide choice label or value, e.g., 'Virtual Agent' or 'virtual_agent')\",\n          \"example\": \"Example Title\"\n        }\n      }\n    },\n    \"note\": {\n      \"type\": \"array\",\n      \"description\": \"List of work notes and comments to add to the ticket\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"Note text\",\n            \"example\": \"example_value\"\n          },\n          \"@type\": {\n            \"type\"\
  : \"string\",\n            \"description\": \"Type of note (determines whether recorded in Work notes or Additional comments field)\",\n            \"example\": \"comments\",\n            \"enum\": [\n              \"comments\",\n              \"work_notes\"\n            ]\n          }\n        },\n        \"required\": [\n          \"text\",\n          \"@type\"\n        ]\n      }\n    },\n    \"relatedEntity\": {\n      \"type\": \"array\",\n      \"description\": \"List of impacted assets, products, sold products, configuration items, or services\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Sys_id of the impacted item or service\",\n            \"example\": \"abc123\"\n          },\n          \"@referredType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of item or service\",\n            \"example\": \"asset\"\
  ,\n            \"enum\": [\n              \"asset\",\n              \"product\",\n              \"product_inventory\",\n              \"cmdb_ci\",\n              \"cmdb_ci_service\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"@referredType\"\n        ]\n      }\n    },\n    \"relatedParty\": {\n      \"type\": \"array\",\n      \"description\": \"Details about contacts for the ticket\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Sys_id of the related party\",\n            \"example\": \"abc123\"\n          },\n          \"@referredType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of related party:\\n- customer: Company or account for the ticket\\n- customer_contact: Caller or contact for the ticket\\n\",\n            \"example\": \"customer\",\n            \"\
  enum\": [\n              \"customer\",\n              \"customer_contact\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"@referredType\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"description\",\n    \"severity\",\n    \"status\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TroubleTicketCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-trouble-ticket-create-schema.json
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
title: TroubleTicketCreate
---
