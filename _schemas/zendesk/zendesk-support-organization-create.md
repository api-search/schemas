---
description: Payload for creating a new organization.
layout: schema
name: OrganizationCreate
properties_list:
- description: The name of the organization.
  name: name
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: notes
  type: string
- description: ''
  name: domain_names
  type: array
- description: ''
  name: group_id
  type: integer
- description: ''
  name: shared_tickets
  type: boolean
- description: ''
  name: shared_comments
  type: boolean
- description: ''
  name: external_id
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: organization_fields
  type: object
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-organization-create-schema.json
slug: zendesk-support-organization-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrganizationCreate\",\n  \"type\": \"object\",\n  \"description\": \"Payload for creating a new organization.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"details\": {\n      \"type\": \"string\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    },\n    \"domain_names\": {\n      \"type\": \"array\"\n    },\n    \"group_id\": {\n      \"type\": \"integer\"\n    },\n    \"shared_tickets\": {\n      \"type\": \"boolean\"\n    },\n    \"shared_comments\": {\n      \"type\": \"boolean\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"organization_fields\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-organization-create-schema.json
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
title: OrganizationCreate
---
