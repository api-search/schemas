---
description: A HubSpot ticket record.
layout: schema
name: Ticket
properties_list:
- description: The unique identifier for the ticket.
  name: id
  type: string
- description: The ticket's properties as key-value pairs.
  name: properties
  type: object
- description: The date and time the ticket was created.
  name: createdAt
  type: string
- description: The date and time the ticket was last updated.
  name: updatedAt
  type: string
- description: Whether the ticket has been archived.
  name: archived
  type: boolean
- description: The ticket's associations with other CRM objects.
  name: associations
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-tickets-api-ticket-schema.json
slug: crm-tickets-api-ticket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-tickets-api-ticket-schema.json\",\n  \"title\": \"Ticket\",\n  \"description\": \"A HubSpot ticket record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the ticket.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The ticket's properties as key-value pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the ticket was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the ticket was last updated.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the ticket has been archived.\",\n      \"example\": true\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"description\": \"The ticket's associations with other CRM objects.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"description\": \"A list of associations.\",\n        \"properties\": {\n          \"results\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Association\"\n            },\n            \"example\": [\n              {\n                \"id\": \"500123\",\n                \"type\": \"standard\"\n              }\n            ]\n          },\n          \"paging\": {\n            \"$ref\": \"#/components/schemas/Paging\"\
  \n          }\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-tickets-api-ticket-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: Ticket
---
