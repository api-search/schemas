---
description: Payload for creating a new ticket.
layout: schema
name: TicketCreate
properties_list:
- description: The subject of the ticket.
  name: subject
  type: string
- description: The initial comment (description) of the ticket.
  name: comment
  type: object
- description: The ID of the requester.
  name: requester_id
  type: integer
- description: Requester details for creating a new user inline. Use either requester_id or requester, not both.
  name: requester
  type: object
- description: The ID of the submitter.
  name: submitter_id
  type: integer
- description: The ID of the assigned agent.
  name: assignee_id
  type: integer
- description: The ID of the assigned group.
  name: group_id
  type: integer
- description: ''
  name: organization_id
  type: integer
- description: ''
  name: type
  type: string
- description: ''
  name: priority
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: external_id
  type: string
- description: ''
  name: custom_fields
  type: array
- description: ''
  name: due_at
  type: string
- description: ''
  name: ticket_form_id
  type: integer
- description: ''
  name: brand_id
  type: integer
- description: ''
  name: collaborator_ids
  type: array
- description: ''
  name: email_cc_ids
  type: array
- description: ''
  name: problem_id
  type: integer
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-ticket-create-schema.json
slug: zendesk-support-ticket-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TicketCreate\",\n  \"type\": \"object\",\n  \"description\": \"Payload for creating a new ticket.\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the ticket.\"\n    },\n    \"comment\": {\n      \"type\": \"object\",\n      \"description\": \"The initial comment (description) of the ticket.\"\n    },\n    \"requester_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the requester.\"\n    },\n    \"requester\": {\n      \"type\": \"object\",\n      \"description\": \"Requester details for creating a new user inline. Use either requester_id or requester, not both.\"\n    },\n    \"submitter_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the submitter.\"\n    },\n    \"assignee_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the assigned agent.\"\n    },\n\
  \    \"group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the assigned group.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    },\n    \"custom_fields\": {\n      \"type\": \"array\"\n    },\n    \"due_at\": {\n      \"type\": \"string\"\n    },\n    \"ticket_form_id\": {\n      \"type\": \"integer\"\n    },\n    \"brand_id\": {\n      \"type\": \"integer\"\n    },\n    \"collaborator_ids\": {\n      \"type\": \"array\"\n    },\n    \"email_cc_ids\": {\n      \"type\": \"array\"\n    },\n    \"problem_id\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-ticket-create-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: TicketCreate
---
