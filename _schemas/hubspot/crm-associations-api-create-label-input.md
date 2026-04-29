---
description: Input for creating an association label
layout: schema
name: CreateLabelInput
properties_list:
- description: Display text for the label
  name: label
  type: string
- description: Internal name for the label
  name: name
  type: string
- description: Label for the inverse direction
  name: inverseLabel
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-create-label-input-schema.json
slug: crm-associations-api-create-label-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-create-label-input-schema.json\",\n  \"title\": \"CreateLabelInput\",\n  \"description\": \"Input for creating an association label\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display text for the label\",\n      \"example\": \"Example Record\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name for the label\",\n      \"example\": \"Example Record\"\n    },\n    \"inverseLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Label for the inverse direction\",\n      \"example\": \"Example Record\"\n    }\n  },\n  \"required\": [\n    \"label\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-create-label-input-schema.json
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
title: CreateLabelInput
---
