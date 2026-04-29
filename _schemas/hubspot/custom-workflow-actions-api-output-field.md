---
description: An output field returned by the action
layout: schema
name: OutputField
properties_list:
- description: Definition of a field's type and configuration
  name: typeDefinition
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-output-field-schema.json
slug: custom-workflow-actions-api-output-field
source_filename: custom-workflow-actions-api-output-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-output-field-schema.json\",\n  \"title\": \"OutputField\",\n  \"description\": \"An output field returned by the action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"Definition of a field's type and configuration\",\n      \"required\": [\n        \"name\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The programmatic name of the field\",\n          \"example\": \"Example Record\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"STRING\",\n            \"NUMBER\",\n            \"BOOL\",\n            \"DATE\",\n            \"DATETIME\",\n            \"ENUMERATION\"\
  ,\n            \"PHONE_NUMBER\",\n            \"CURRENCY\"\n          ],\n          \"description\": \"The data type of the field\",\n          \"example\": \"STRING\"\n        },\n        \"fieldType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"TEXT\",\n            \"TEXTAREA\",\n            \"NUMBER\",\n            \"SELECT\",\n            \"BOOLEANCHECKBOX\",\n            \"DATE\",\n            \"FILE\"\n          ],\n          \"description\": \"The UI field type for input\",\n          \"example\": \"TEXT\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable label for the field\",\n          \"example\": \"Example Record\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the field\",\n          \"example\": \"This is an example description.\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"\
  description\": \"Options for enumeration fields\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/FieldOption\"\n          },\n          \"example\": [\n            {\n              \"label\": \"Example Record\",\n              \"value\": \"example-value\",\n              \"displayOrder\": 100\n            }\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"typeDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-output-field-schema.json
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
title: OutputField
---
