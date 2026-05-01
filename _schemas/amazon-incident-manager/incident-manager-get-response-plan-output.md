---
description: GetResponsePlanOutput schema
layout: schema
name: GetResponsePlanOutput
properties_list:
- description: ''
  name: actions
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: chatChannel
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: engagements
  type: object
- description: ''
  name: incidentTemplate
  type: object
- description: ''
  name: integrations
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-get-response-plan-output-schema.json
slug: incident-manager-get-response-plan-output
source_filename: incident-manager-get-response-plan-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-response-plan-output-schema.json\",\n  \"title\": \"GetResponsePlanOutput\",\n  \"description\": \"GetResponsePlanOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"The actions that this response plan takes at the beginning of the incident.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the response plan.\"\n        }\n      ]\n    },\n    \"chatChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChatChannel\"\n        },\n  \
  \      {\n          \"description\": \"The Chatbot chat channel used for collaboration during an incident.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponsePlanDisplayName\"\n        },\n        {\n          \"description\": \"The long format name of the response plan. Can contain spaces.\"\n        }\n      ]\n    },\n    \"engagements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngagementSet\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the contacts and escalation plans that the response plan engages during an incident.\"\n        }\n      ]\n    },\n    \"incidentTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTemplate\"\n        },\n        {\n          \"description\": \"Details used to create the incident when using this response plan.\"\n        }\n      ]\n    },\n\
  \    \"integrations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integrations\"\n        },\n        {\n          \"description\": \"Information about third-party services integrated into the Incident Manager response plan.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponsePlanName\"\n        },\n        {\n          \"description\": \"The short format name of the response plan. The name can't contain spaces.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"incidentTemplate\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-get-response-plan-output-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: GetResponsePlanOutput
---
