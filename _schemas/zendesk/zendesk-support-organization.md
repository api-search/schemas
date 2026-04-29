---
description: A Zendesk organization representing a company or group of users.
layout: schema
name: Organization
properties_list:
- description: Automatically assigned organization ID.
  name: id
  type: integer
- description: The API URL of the organization.
  name: url
  type: string
- description: The name of the organization.
  name: name
  type: string
- description: Details about the organization.
  name: details
  type: string
- description: Notes about the organization visible only to agents.
  name: notes
  type: string
- description: Domain names associated with the organization. Users with matching email domains can be auto-assigned.
  name: domain_names
  type: array
- description: The default group assigned to tickets from this organization.
  name: group_id
  type: integer
- description: Whether end users in the organization can see each other's tickets.
  name: shared_tickets
  type: boolean
- description: Whether end users in the organization can see each other's comments on tickets.
  name: shared_comments
  type: boolean
- description: An external ID from an integrated system.
  name: external_id
  type: string
- description: Tags applied to the organization.
  name: tags
  type: array
- description: Custom organization field values (key-value pairs).
  name: organization_fields
  type: object
- description: When the organization was created (ISO 8601).
  name: created_at
  type: string
- description: When the organization was last updated (ISO 8601).
  name: updated_at
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-organization-schema.json
slug: zendesk-support-organization
source_filename: zendesk-support-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"description\": \"A Zendesk organization representing a company or group of users.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Automatically assigned organization ID.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The API URL of the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Details about the organization.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes about the organization visible only to agents.\"\n    },\n    \"domain_names\": {\n      \"type\": \"array\",\n      \"description\": \"Domain names associated with the organization. Users with matching email\
  \ domains can be auto-assigned.\"\n    },\n    \"group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The default group assigned to tickets from this organization.\"\n    },\n    \"shared_tickets\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether end users in the organization can see each other's tickets.\"\n    },\n    \"shared_comments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether end users in the organization can see each other's comments on tickets.\"\n    },\n    \"external_id\": {\n      \"type\": \"string\",\n      \"description\": \"An external ID from an integrated system.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the organization.\"\n    },\n    \"organization_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom organization field values (key-value pairs).\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"\
  When the organization was created (ISO 8601).\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the organization was last updated (ISO 8601).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-organization-schema.json
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
title: Organization
---
