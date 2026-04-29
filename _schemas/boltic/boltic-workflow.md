---
description: A Boltic automation workflow consisting of triggers, nodes, and execution configuration for orchestrating tasks across integrations.
layout: schema
name: Boltic Workflow
properties_list:
- description: Unique identifier for the workflow
  name: id
  type: string
- description: Human-readable name for the workflow
  name: name
  type: string
- description: Description of what the workflow does
  name: description
  type: string
- description: Current status of the workflow
  name: status
  type: string
- description: ''
  name: trigger
  type: object
- description: Ordered list of action nodes in the workflow
  name: nodes
  type: array
- description: Tags for categorizing the workflow
  name: tags
  type: array
- description: Total number of times this workflow has been executed
  name: executionCount
  type: integer
- description: Timestamp of the last execution
  name: lastExecutedAt
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-workflow.json
slug: boltic-workflow
source_filename: boltic-workflow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-workflow.json\",\n  \"title\": \"Boltic Workflow\",\n  \"description\": \"A Boltic automation workflow consisting of triggers, nodes, and execution configuration for orchestrating tasks across integrations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"trigger\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workflow\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the workflow\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the workflow does\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"draft\"],\n      \"description\": \"Current\
  \ status of the workflow\"\n    },\n    \"trigger\": {\n      \"$ref\": \"#/$defs/trigger\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/node\"\n      },\n      \"description\": \"Ordered list of action nodes in the workflow\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for categorizing the workflow\"\n    },\n    \"executionCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of times this workflow has been executed\"\n    },\n    \"lastExecutedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last execution\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\":\
  \ {\n    \"trigger\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"http\", \"schedule\", \"webhook\", \"copilot\", \"table-change\", \"manual\"],\n          \"description\": \"Type of trigger that initiates the workflow\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Trigger-specific configuration\"\n        },\n        \"methods\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\"]\n          },\n          \"description\": \"HTTP methods for HTTP triggers\"\n        }\n      }\n    },\n    \"node\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"name\"],\n      \"properties\": {\n       \
  \ \"id\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"integration\", \"transformation\", \"destination\", \"condition\", \"loop\", \"ai\"],\n          \"description\": \"Type of workflow node\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"integrationId\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to the integration this node uses\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"position\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"x\": { \"type\": \"number\" },\n            \"y\": { \"type\": \"number\" }\n          }\n        },\n        \"connections\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"targetNodeId\": {\
  \ \"type\": \"string\" },\n              \"condition\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-workflow.json
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Workflow
---
