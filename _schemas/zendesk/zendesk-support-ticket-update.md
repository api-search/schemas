---
description: Payload for updating an existing ticket.
layout: schema
name: TicketUpdate
properties_list:
- description: ''
  name: subject
  type: string
- description: A new comment to add to the ticket.
  name: comment
  type: object
- description: ''
  name: assignee_id
  type: integer
- description: ''
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
  name: custom_fields
  type: array
- description: ''
  name: due_at
  type: string
- description: ''
  name: problem_id
  type: integer
- description: ''
  name: collaborator_ids
  type: array
- description: ''
  name: email_cc_ids
  type: array
- description: ''
  name: external_id
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-ticket-update-schema.json
slug: zendesk-support-ticket-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TicketUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Payload for updating an existing ticket.\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"object\",\n      \"description\": \"A new comment to add to the ticket.\"\n    },\n    \"assignee_id\": {\n      \"type\": \"integer\"\n    },\n    \"group_id\": {\n      \"type\": \"integer\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"custom_fields\": {\n      \"type\": \"array\"\n    },\n    \"due_at\": {\n      \"type\": \"string\"\n    },\n    \"problem_id\": {\n      \"type\": \"integer\"\n    },\n    \"collaborator_ids\"\
  : {\n      \"type\": \"array\"\n    },\n    \"email_cc_ids\": {\n      \"type\": \"array\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-ticket-update-schema.json
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
title: TicketUpdate
---
