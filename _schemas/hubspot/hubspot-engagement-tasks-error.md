---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: correlationId
  type: string
- description: ''
  name: category
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-tasks-error-schema.json
slug: hubspot-engagement-tasks-error
source_filename: hubspot-engagement-tasks-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-tasks-error-schema.json
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
title: Error
---
