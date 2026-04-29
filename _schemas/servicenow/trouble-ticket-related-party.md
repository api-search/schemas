---
description: ''
layout: schema
name: RelatedParty
properties_list:
- description: Sys_id of the related party
  name: id
  type: string
- description: Name of the related party
  name: name
  type: string
- description: 'Type of related party: - assigned_to: User assigned to work on the ticket - assignment_group: Group assigned to work on the ticket - customer: Company or account for the ticket - customer_contact: Cal'
  name: '@referredType'
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-related-party-schema.json
slug: trouble-ticket-related-party
source_filename: trouble-ticket-related-party-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the related party\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the related party\",\n      \"example\": \"Example Title\"\n    },\n    \"@referredType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of related party:\\n- assigned_to: User assigned to work on the ticket\\n- assignment_group: Group assigned to work on the ticket\\n- customer: Company or account for the ticket\\n- customer_contact: Caller or contact for the ticket\\n\",\n      \"example\": \"assigned_to\",\n      \"enum\": [\n        \"assigned_to\",\n        \"assignment_group\",\n        \"customer\",\n        \"customer_contact\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedParty\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-related-party-schema.json
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
title: RelatedParty
---
