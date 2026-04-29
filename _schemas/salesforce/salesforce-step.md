---
description: ''
layout: schema
name: Step
properties_list:
- description: ''
  name: actionType
  type: string
- description: ''
  name: assignment
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: resultIncluded
  type: boolean
- description: ''
  name: sequenceNumber
  type: integer
- description: ''
  name: shouldExposeConditionDetails
  type: boolean
- description: ''
  name: shouldExposeExecPathMsgOnly
  type: boolean
- description: ''
  name: shouldShowExplExternally
  type: boolean
- description: ''
  name: stepType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-step-schema.json
slug: salesforce-step
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"assignment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"assignedParameter\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expression\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"assignedParameter\",\n        \"expression\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"resultIncluded\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"shouldExposeConditionDetails\": {\n     \
  \ \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"shouldExposeExecPathMsgOnly\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"shouldShowExplExternally\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"stepType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"actionType\",\n    \"assignment\",\n    \"description\",\n    \"name\",\n    \"resultIncluded\",\n    \"sequenceNumber\",\n    \"shouldExposeConditionDetails\",\n    \"shouldExposeExecPathMsgOnly\",\n    \"shouldShowExplExternally\",\n    \"stepType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Step\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-step-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Step
---
