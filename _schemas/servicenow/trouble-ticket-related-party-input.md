---
description: ''
layout: schema
name: RelatedPartyInput
properties_list:
- description: Sys_id of the related party
  name: id
  type: string
- description: 'Type of related party: - customer: Company or account for the ticket - customer_contact: Caller or contact for the ticket'
  name: '@referredType'
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/trouble-ticket-related-party-input-schema.json
slug: trouble-ticket-related-party-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the related party\",\n      \"example\": \"abc123\"\n    },\n    \"@referredType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of related party:\\n- customer: Company or account for the ticket\\n- customer_contact: Caller or contact for the ticket\\n\",\n      \"example\": \"customer\",\n      \"enum\": [\n        \"customer\",\n        \"customer_contact\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"@referredType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedPartyInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/trouble-ticket-related-party-input-schema.json
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
title: RelatedPartyInput
---
