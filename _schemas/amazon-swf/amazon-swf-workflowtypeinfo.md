---
description: Contains information about a workflow type.
layout: schema
name: WorkflowTypeInfo
properties_list:
- description: ''
  name: workflowType
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: deprecationDate
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowtypeinfo-schema.json
slug: amazon-swf-workflowtypeinfo
source_filename: amazon-swf-workflowtypeinfo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowType\",\n    \"status\",\n    \"creationDate\"\n  ],\n  \"properties\": {\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The workflow type this information is about.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"The current status of the workflow type.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the type registered through <a>RegisterWorkflowType</a>.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The date when this type was registered.\"\n        }\n      ]\n    },\n    \"deprecationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If the type is in deprecated state, then it is set to the date when the type was deprecated.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains information about a workflow type.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowTypeInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowtypeinfo-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: WorkflowTypeInfo
---
