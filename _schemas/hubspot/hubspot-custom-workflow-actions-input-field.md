---
description: An input field for the action
layout: schema
name: InputField
properties_list:
- description: Definition of a field's type and configuration
  name: typeDefinition
  type: object
- description: The types of values that can be provided for this field
  name: supportedValueTypes
  type: array
- description: Whether this field is required
  name: isRequired
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-input-field-schema.json
slug: hubspot-custom-workflow-actions-input-field
source_filename: hubspot-custom-workflow-actions-input-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An input field for the action\",\n  \"properties\": {\n    \"typeDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"Definition of a field's type and configuration\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The programmatic name of the field\",\n          \"example\": \"Example Record\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the field\",\n          \"example\": \"STRING\",\n          \"enum\": [\n            \"STRING\",\n            \"NUMBER\",\n            \"BOOL\",\n            \"DATE\",\n            \"DATETIME\",\n            \"ENUMERATION\",\n            \"PHONE_NUMBER\",\n            \"CURRENCY\"\n          ]\n        },\n        \"fieldType\": {\n          \"type\": \"string\",\n          \"description\": \"The UI field type for input\",\n          \"example\"\
  : \"TEXT\",\n          \"enum\": [\n            \"TEXT\",\n            \"TEXTAREA\",\n            \"NUMBER\",\n            \"SELECT\",\n            \"BOOLEANCHECKBOX\",\n            \"DATE\",\n            \"FILE\"\n          ]\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable label for the field\",\n          \"example\": \"Example Record\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the field\",\n          \"example\": \"This is an example description.\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"description\": \"Options for enumeration fields\",\n          \"example\": [\n            {\n              \"label\": \"Example Record\",\n              \"value\": \"example-value\",\n              \"displayOrder\": 100\n            }\n          ],\n          \"items\": {\n            \"type\": \"object\",\n            \"\
  description\": \"An option for an enumeration field\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\",\n                \"description\": \"Display label for the option\",\n                \"example\": \"Example Record\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"The value of the option\",\n                \"example\": \"example-value\"\n              },\n              \"displayOrder\": {\n                \"type\": \"integer\",\n                \"description\": \"Order in which to display the option\",\n                \"example\": 100\n              }\n            },\n            \"required\": [\n              \"label\",\n              \"value\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"type\"\n      ]\n    },\n    \"supportedValueTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The types\
  \ of values that can be provided for this field\",\n      \"example\": [\n        \"STATIC_VALUE\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"STATIC_VALUE\",\n          \"OBJECT_PROPERTY\",\n          \"OUTPUT_FROM_PREVIOUS_ACTION\"\n        ]\n      }\n    },\n    \"isRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this field is required\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"typeDefinition\",\n    \"supportedValueTypes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InputField\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-input-field-schema.json
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
title: InputField
---
