---
description: Request body for updating a note
layout: schema
name: NoteUpdateRequest
properties_list:
- description: The note properties to update
  name: properties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-note-update-request-schema.json
slug: hubspot-engagement-notes-note-update-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a note\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The note properties to update\",\n      \"example\": {\n        \"hs_note_body\": \"Updated meeting notes - client confirmed interest in premium tier.\"\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoteUpdateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-note-update-request-schema.json
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
title: NoteUpdateRequest
---
