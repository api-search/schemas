---
description: Represents an audit event for activities performed by users on the Productiv platform.
layout: schema
name: AuditEvent
properties_list:
- description: The unique identifier of the event.
  name: eventId
  type: string
- description: The type of audit event.
  name: eventType
  type: string
- description: When the event occurred.
  name: timestamp
  type: string
- description: The email of the user who performed the action.
  name: userEmail
  type: string
- description: Additional details about the event.
  name: details
  type: object
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/audit-event.json
slug: audit-event
source_filename: audit-event.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"audit-event.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuditEvent\",\n  \"description\": \"Represents an audit event for activities performed by users on the Productiv platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the event.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of audit event.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the event occurred.\"\n    },\n    \"userEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email of the user who performed the action.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional details about the event.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/audit-event.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: AuditEvent
---
