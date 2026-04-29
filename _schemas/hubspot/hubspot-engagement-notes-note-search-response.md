---
description: Search results for notes
layout: schema
name: NoteSearchResponse
properties_list:
- description: Total number of matching notes
  name: total
  type: integer
- description: The matching notes
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-note-search-response-schema.json
slug: hubspot-engagement-notes-note-search-response
source_filename: hubspot-engagement-notes-note-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Search results for notes\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching notes\",\n      \"example\": 42\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The matching notes\",\n      \"example\": [\n        {\n          \"id\": \"1024\",\n          \"properties\": {\n            \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n            \"hubspot_owner_id\": \"12345\"\n          },\n          \"propertiesWithHistory\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2024-01-15T10:30:00.000Z\",\n          \"updatedAt\": \"2024-01-15T11:00:00.000Z\",\n          \"archived\": false,\n          \"archivedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ],\n      \"items\"\
  : {\n        \"type\": \"object\",\n        \"description\": \"Represents a note engagement in the CRM\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the note\",\n            \"example\": \"1024\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The note properties\",\n            \"example\": {\n              \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n              \"hubspot_owner_id\": \"12345\"\n            }\n          },\n          \"propertiesWithHistory\": {\n            \"type\": \"object\",\n            \"description\": \"Properties with their change history\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n          \
  \  \"type\": \"string\",\n            \"description\": \"When the note was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T10:30:00.000Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the note was last updated\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T11:00:00.000Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the note is archived\",\n            \"example\": false\n          },\n          \"archivedAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the note was archived (if archived)\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"properties\",\n          \"createdAt\",\n          \"updatedAt\",\n          \"archived\"\
  \n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Information about the next page\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\",\n              \"example\": \"MTAyNA%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          },\n          \"required\": [\n            \"after\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"total\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoteSearchResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-note-search-response-schema.json
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
title: NoteSearchResponse
---
