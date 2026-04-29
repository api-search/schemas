---
description: Represents a note engagement in the CRM
layout: schema
name: Note
properties_list:
- description: The unique identifier for the note
  name: id
  type: string
- description: The note properties
  name: properties
  type: object
- description: Properties with their change history
  name: propertiesWithHistory
  type: object
- description: When the note was created
  name: createdAt
  type: string
- description: When the note was last updated
  name: updatedAt
  type: string
- description: Whether the note is archived
  name: archived
  type: boolean
- description: When the note was archived (if archived)
  name: archivedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-notes-note-schema.json
slug: engagement-notes-note
source_filename: engagement-notes-note-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-note-schema.json\",\n  \"title\": \"Note\",\n  \"description\": \"Represents a note engagement in the CRM\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the note\",\n      \"example\": \"1024\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The note properties\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n        \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n        \"hubspot_owner_id\": \"12345\"\n      }\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"object\",\n    \
  \  \"description\": \"Properties with their change history\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"description\": \"Historical value of a property\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"description\": \"The historical value\",\n              \"example\": \"Initial meeting notes\"\n            },\n            \"timestamp\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"When the value was set\",\n              \"example\": \"2024-01-15T10:30:00.000Z\"\n            },\n            \"sourceType\": {\n              \"type\": \"string\",\n              \"description\": \"The source type that set this value\",\n              \"example\": \"CRM_UI\"\n            },\n            \"sourceId\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"The source identifier\",\n              \"example\": \"userId:12345\"\n            },\n            \"sourceLabel\": {\n              \"type\": \"string\",\n              \"description\": \"Human-readable source label\",\n              \"example\": \"John Doe\"\n            },\n            \"updatedByUserId\": {\n              \"type\": \"integer\",\n              \"description\": \"The user ID who made the change\",\n              \"example\": 12345\n            }\n          }\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the note was created\",\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the note was last updated\",\n      \"example\": \"2024-01-15T11:00:00.000Z\"\n    },\n    \"archived\": {\n    \
  \  \"type\": \"boolean\",\n      \"description\": \"Whether the note is archived\",\n      \"example\": false\n    },\n    \"archivedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the note was archived (if archived)\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"properties\",\n    \"createdAt\",\n    \"updatedAt\",\n    \"archived\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-note-schema.json
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
title: Note
---
