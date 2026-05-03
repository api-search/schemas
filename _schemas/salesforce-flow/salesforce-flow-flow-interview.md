---
description: Schema for a Salesforce Flow Interview, representing a running instance of a Flow.
layout: schema
name: Salesforce Flow Interview
properties_list:
- description: Salesforce record ID for the FlowInterview
  name: Id
  type: string
- description: Auto-generated name for the interview
  name: Name
  type: string
- description: API name of the current flow element being executed
  name: CurrentElement
  type: string
- description: API name of the Flow being interviewed
  name: GuidedFlowName
  type: string
- description: Whether the flow interview has completed
  name: HasFinished
  type: boolean
- description: Salesforce ID of the interview owner
  name: OwnerId
  type: string
- description: Label for the pause element if flow is paused
  name: PauseLabel
  type: string
- description: Timestamp when the interview was created
  name: CreatedDate
  type: string
- description: Timestamp when the interview was last modified
  name: LastModifiedDate
  type: string
- description: Input variables passed to the flow interview
  name: inputs
  type: array
- description: Output variables returned by the flow interview
  name: outputs
  type: array
provider_name: Salesforce Flow
provider_slug: salesforce-flow
schema_file: json-schema/salesforce-flow-flow-interview-schema.json
slug: salesforce-flow-flow-interview
source_filename: salesforce-flow-flow-interview-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-flow/blob/main/json-schema/salesforce-flow-flow-interview-schema.json\",\n  \"title\": \"Salesforce Flow Interview\",\n  \"description\": \"Schema for a Salesforce Flow Interview, representing a running instance of a Flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID for the FlowInterview\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated name for the interview\"\n    },\n    \"CurrentElement\": {\n      \"type\": \"string\",\n      \"description\": \"API name of the current flow element being executed\"\n    },\n    \"GuidedFlowName\": {\n      \"type\": \"string\",\n      \"description\": \"API name of the Flow being interviewed\"\n    },\n    \"HasFinished\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the flow interview has completed\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the interview owner\"\n    },\n    \"PauseLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Label for the pause element if flow is paused\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the interview was created\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the interview was last modified\"\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Input variables passed to the flow interview\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Variable name\"\n          },\n          \"value\": {\n     \
  \       \"description\": \"Variable value\"\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"description\": \"Output variables returned by the flow interview\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Variable name\"\n          },\n          \"value\": {\n            \"description\": \"Variable value\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"Id\", \"GuidedFlowName\", \"HasFinished\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/json-schema/salesforce-flow-flow-interview-schema.json
tags:
- Automation
- Business Process
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
title: Salesforce Flow Interview
---
