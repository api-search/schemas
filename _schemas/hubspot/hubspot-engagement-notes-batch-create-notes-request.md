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
schema_file: json-schema/hubspot-engagement-notes-batch-create-notes-request-schema.json
slug: hubspot-engagement-notes-batch-create-notes-request
source_filename: hubspot-engagement-notes-batch-create-notes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch creating notes\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of notes to create\",\n      \"example\": [\n        {\n          \"properties\": {\n            \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n            \"hubspot_owner_id\": \"12345\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Request body for creating a note\",\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"\
  The note properties to set\",\n            \"example\": {\n              \"hs_note_body\": \"Met with client to discuss Q1 goals. They are interested in expanding their subscription.\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\",\n              \"hubspot_owner_id\": \"12345\"\n            }\n          },\n          \"associations\": {\n            \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Association to create with another object\",\n              \"properties\": {\n                \"to\": {\n                  \"type\": \"object\",\n                  \"example\": {\n                    \"id\": \"\
  101\"\n                  },\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\"\n                  ]\n                },\n                \"types\": {\n                  \"type\": \"array\",\n                  \"description\": \"The association types\",\n                  \"example\": [\n                    {\n                      \"associationCategory\": \"HUBSPOT_DEFINED\",\n                      \"associationTypeId\": 202\n                    }\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"to\",\n                \"types\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"properties\"\n        ]\n      }\n    }\n  },\n\
  \  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCreateNotesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-create-notes-request-schema.json
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
