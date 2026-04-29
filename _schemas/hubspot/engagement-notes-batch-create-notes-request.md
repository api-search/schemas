---
description: Request body for batch creating notes
layout: schema
name: BatchCreateNotesRequest
properties_list:
- description: Array of notes to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-notes-batch-create-notes-request-schema.json
slug: engagement-notes-batch-create-notes-request
source_filename: engagement-notes-batch-create-notes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-batch-create-notes-request-schema.json\",\n  \"title\": \"BatchCreateNotesRequest\",\n  \"description\": \"Request body for batch creating notes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of notes to create\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Request body for creating a note\",\n        \"required\": [\n          \"properties\"\n        ],\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The note properties to set\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"hs_note_body\": \"Met with client to discuss\
  \ Q1 goals. They are interested in expanding their subscription.\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n              \"hubspot_owner_id\": \"12345\"\n            }\n          },\n          \"associations\": {\n            \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationInput\"\n            },\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ]\n          }\n        }\n      },\n      \"maxItems\": 100,\n      \"example\": [\n        {\n          \"properties\": {\n            \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n      \
  \      \"hubspot_owner_id\": \"12345\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-notes-batch-create-notes-request-schema.json
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
title: BatchCreateNotesRequest
---
