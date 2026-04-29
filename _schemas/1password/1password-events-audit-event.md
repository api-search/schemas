---
description: Represents an audit event recording an action performed by a team member within the 1Password account.
layout: schema
name: AuditEvent
properties_list:
- description: The unique identifier for the audit event.
  name: uuid
  type: string
- description: When the action was performed.
  name: timestamp
  type: string
- description: The UUID of the user who performed the action.
  name: actor_uuid
  type: string
- description: ''
  name: actor_details
  type: object
- description: The type of action that was performed.
  name: action
  type: string
- description: The type of object the action was performed on.
  name: object_type
  type: string
- description: The UUID of the object the action was performed on.
  name: object_uuid
  type: string
- description: Additional details about the object of the action.
  name: object_details
  type: object
- description: An auxiliary identifier providing additional context.
  name: aux_id
  type: integer
- description: An auxiliary UUID providing additional context.
  name: aux_uuid
  type: string
- description: Additional auxiliary details about the event.
  name: aux_details
  type: object
- description: Additional auxiliary information about the event.
  name: aux_info
  type: string
- description: Information about the session in which the action occurred.
  name: session
  type: object
- description: ''
  name: location
  type: object
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-audit-event-schema.json
slug: 1password-events-audit-event
source_filename: 1password-events-audit-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-audit-event-schema.json\",\n  \"title\": \"AuditEvent\",\n  \"description\": \"Represents an audit event recording an action performed by a team member within the 1Password account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the audit event.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the action was performed.\"\n    },\n    \"actor_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the user who performed the action.\"\n    },\n    \"actor_details\": {\n      \"$ref\": \"#/components/schemas/EventUser\"\n    },\n    \"action\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The type of action that was performed.\"\n    },\n    \"object_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of object the action was performed on.\"\n    },\n    \"object_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the object the action was performed on.\"\n    },\n    \"object_details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional details about the object of the action.\"\n    },\n    \"aux_id\": {\n      \"type\": \"integer\",\n      \"description\": \"An auxiliary identifier providing additional context.\"\n    },\n    \"aux_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"An auxiliary UUID providing additional context.\"\n    },\n    \"aux_details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional auxiliary details about the event.\"\n    },\n   \
  \ \"aux_info\": {\n      \"type\": \"string\",\n      \"description\": \"Additional auxiliary information about the event.\"\n    },\n    \"session\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the session in which the action occurred.\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The UUID of the session.\"\n        },\n        \"login_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the session was created.\"\n        },\n        \"device_uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The UUID of the device used.\"\n        },\n        \"ip\": {\n          \"type\": \"string\",\n          \"description\": \"The IP address of the client.\"\n        }\n      }\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/EventLocation\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-audit-event-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: AuditEvent
---
