---
description: An option for an enumeration field
layout: schema
name: FieldOption
properties_list:
- description: Display label for the option
  name: label
  type: string
- description: The value of the option
  name: value
  type: string
- description: Order in which to display the option
  name: displayOrder
  type: integer
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-field-option-schema.json
slug: custom-workflow-actions-api-field-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-field-option-schema.json\",\n  \"title\": \"FieldOption\",\n  \"description\": \"An option for an enumeration field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label for the option\",\n      \"example\": \"Example Record\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the option\",\n      \"example\": \"example-value\"\n    },\n    \"displayOrder\": {\n      \"type\": \"integer\",\n      \"description\": \"Order in which to display the option\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"label\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-field-option-schema.json
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
title: FieldOption
---
