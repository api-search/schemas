---
description: CreateResponsePlanInput schema
layout: schema
name: CreateResponsePlanInput
properties_list:
- description: ''
  name: actions
  type: object
- description: ''
  name: chatChannel
  type: object
- description: ''
  name: clientToken
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
- description: ''
  name: tags
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-create-response-plan-input-schema.json
slug: incident-manager-create-response-plan-input
source_filename: incident-manager-create-response-plan-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-response-plan-input-schema.json\",\n  \"title\": \"CreateResponsePlanInput\",\n  \"description\": \"CreateResponsePlanInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"The actions that the response plan starts at the beginning of an incident.\"\n        }\n      ]\n    },\n    \"chatChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChatChannel\"\n        },\n        {\n          \"description\": \"The Chatbot chat channel used for collaboration during an incident.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token ensuring that the operation is called only once with the specified details.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponsePlanDisplayName\"\n        },\n        {\n          \"description\": \"The long format of the response plan name. This field can contain spaces.\"\n        }\n      ]\n    },\n    \"engagements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngagementSet\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the contacts and escalation plans that the response plan engages during an incident.\"\n        }\n      ]\n    },\n    \"incidentTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTemplate\"\n        },\n        {\n          \"description\": \"Details used to create\
  \ an incident when using this response plan.\"\n        }\n      ]\n    },\n    \"integrations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integrations\"\n        },\n        {\n          \"description\": \"Information about third-party services integrated into the response plan.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponsePlanName\"\n        },\n        {\n          \"description\": \"The short format name of the response plan. Can't include spaces.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags that you are adding to the response plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentTemplate\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-create-response-plan-input-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: CreateResponsePlanInput
---
