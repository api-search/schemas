---
description: ''
layout: schema
name: TroubleTicket
properties_list:
- description: This value is always TroubleTicket
  name: '@type'
  type: string
- description: The sys_id of the case or incident record
  name: id
  type: string
- description: Relative link to the case or incident record
  name: href
  type: string
- description: The date that the case or incident record was created
  name: creationDate
  type: string
- description: The date the record was last updated
  name: lastUpdate
  type: string
- description: The name of the trouble ticket, typically a short description of the issue
  name: name
  type: string
- description: The description of the issue from the ticket
  name: description
  type: string
- description: The severity of the issue described by the trouble ticket
  name: severity
  type: string
- description: The current status of the trouble ticket
  name: status
  type: string
- description: The type of ticket
  name: ticketType
  type: string
- description: ''
  name: channel
  type: object
- description: A list of all comments on the ticket (excludes work notes)
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
schema_file: json-schema/trouble-ticket-trouble-ticket-schema.json
slug: trouble-ticket-trouble-ticket
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"This value is always TroubleTicket\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the case or incident record\",\n      \"example\": \"abc123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Relative link to the case or incident record\",\n      \"example\": \"example_value\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date that the case or incident record was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"lastUpdate\": {\n      \"type\": \"string\",\n      \"description\": \"The date the record was last updated\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"name\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The name of the trouble ticket, typically a short description of the issue\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the issue from the ticket\",\n      \"example\": \"A sample description.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity of the issue described by the trouble ticket\",\n      \"example\": \"2 - High\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the trouble ticket\",\n      \"example\": \"example_value\"\n    },\n    \"ticketType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of ticket\",\n      \"example\": \"Case\",\n      \"enum\": [\n        \"Case\",\n        \"Incident\",\n        \"Service Problem Case\"\n      ]\n    },\n    \"channel\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the contact method\",\n          \"example\": \"Example Title\"\n        }\n      }\n    },\n    \"note\": {\n      \"type\": \"array\",\n      \"description\": \"A list of all comments on the ticket (excludes work notes)\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"@type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of note (always 'comments' in responses)\",\n            \"example\": \"example_value\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"The comment text\",\n            \"example\": \"example_value\"\n          },\n          \"date\": {\n            \"type\": \"string\",\n            \"description\": \"The date the comment was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2026-01-15T10:30:00Z\"\
  \n          },\n          \"author\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the user who wrote the comment\",\n            \"example\": \"example_value\"\n          }\n        }\n      }\n    },\n    \"relatedEntity\": {\n      \"type\": \"array\",\n      \"description\": \"List of impacted assets, products, sold products, configuration items, or services\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"@type\": {\n            \"type\": \"string\",\n            \"description\": \"This value is always relatedEntity\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Sys_id of the impacted item or service\",\n            \"example\": \"abc123\"\n          },\n          \"href\": {\n            \"type\": \"string\",\n            \"description\": \"Returns an empty string\",\n       \
  \     \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the impacted item or service\",\n            \"example\": \"Example Title\"\n          },\n          \"role\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the impacted item or service\",\n            \"example\": \"example_value\"\n          },\n          \"@referredType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of item or service\",\n            \"example\": \"asset\",\n            \"enum\": [\n              \"asset\",\n              \"product\",\n              \"product_inventory\",\n              \"cmdb_ci\",\n              \"cmdb_ci_service\"\n            ]\n          }\n        }\n      }\n    },\n    \"relatedParty\": {\n      \"type\": \"array\",\n      \"description\": \"Details about contacts for the ticket\",\n      \"example\": [],\n      \"items\": {\n \
  \       \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Sys_id of the related party\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the related party\",\n            \"example\": \"Example Title\"\n          },\n          \"@referredType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of related party:\\n- assigned_to: User assigned to work on the ticket\\n- assignment_group: Group assigned to work on the ticket\\n- customer: Company or account for the ticket\\n- customer_contact: Caller or contact for the ticket\\n\",\n            \"example\": \"assigned_to\",\n            \"enum\": [\n              \"assigned_to\",\n              \"assignment_group\",\n              \"customer\",\n              \"customer_contact\"\n            ]\n          }\n        }\n      }\n \
  \   }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TroubleTicket\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-trouble-ticket-schema.json
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
title: TroubleTicket
---
