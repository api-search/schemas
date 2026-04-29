---
description: ''
layout: schema
name: Campaign
properties_list:
- description: Unique identifier for the campaign.
  name: id
  type: integer
- description: Name of the campaign.
  name: name
  type: string
- description: Number of recipients in the campaign.
  name: recipients_count
  type: integer
- description: Whether the campaign can be edited.
  name: editable
  type: boolean
- description: Whether the campaign has been started.
  name: started
  type: boolean
- description: Whether the campaign has been archived.
  name: archived
  type: boolean
- description: Whether the campaign is paused.
  name: paused
  type: boolean
- description: Current sending status of the campaign.
  name: sending_status
  type: '[''string'', ''null'']'
- description: Timestamp when the campaign was created.
  name: created_at
  type: string
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-campaign-schema.json
slug: hunter-campaign
source_filename: hunter-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Campaign\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the campaign.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the campaign.\"\n    },\n    \"recipients_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of recipients in the campaign.\"\n    },\n    \"editable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign can be edited.\"\n    },\n    \"started\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign has been started.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign has been archived.\"\n    },\n    \"paused\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign is paused.\"\n    },\n\
  \    \"sending_status\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Current sending status of the campaign.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the campaign was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-campaign-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: Campaign
---
