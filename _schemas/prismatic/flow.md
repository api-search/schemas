---
description: A flow is a sequence of steps within an integration that defines a specific workflow or automation path, including triggers and actions.
layout: schema
name: Prismatic Flow
properties_list:
- description: Unique identifier for the flow
  name: id
  type: string
- description: Name of the flow
  name: name
  type: string
- description: Description of what the flow does
  name: description
  type: string
- description: Stable key used to reference the flow across versions
  name: stableKey
  type: string
- description: Whether the flow runs synchronously and returns a response
  name: isSynchronous
  type: boolean
- description: Maximum number of retry attempts on failure
  name: retryMaxAttempts
  type: integer
- description: Delay in minutes between retry attempts
  name: retryDelayMinutes
  type: integer
- description: Field used as unique request ID for deduplication
  name: retryUniqueRequestIdField
  type: string
- description: Security type for the flow webhook endpoint
  name: endpointSecurityType
  type: string
- description: Ordered list of steps in the flow
  name: steps
  type: array
- description: Timestamp when the flow was created
  name: createdAt
  type: string
- description: Timestamp when the flow was last updated
  name: updatedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/flow.json
slug: flow
source_filename: flow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/flow.json\",\n  \"title\": \"Prismatic Flow\",\n  \"description\": \"A flow is a sequence of steps within an integration that defines a specific workflow or automation path, including triggers and actions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the flow\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the flow\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the flow does\"\n    },\n    \"stableKey\": {\n      \"type\": \"string\",\n      \"description\": \"Stable key used to reference the flow across versions\"\n    },\n    \"isSynchronous\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the flow runs synchronously and returns a response\"\n    },\n    \"retryMaxAttempts\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of retry attempts on failure\"\n    },\n    \"retryDelayMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay in minutes between retry attempts\"\n    },\n    \"retryUniqueRequestIdField\": {\n      \"type\": \"string\",\n      \"description\": \"Field used as unique request ID for deduplication\"\n    },\n    \"endpointSecurityType\": {\n      \"type\": \"string\",\n      \"enum\": [\"customer_optional\", \"customer_required\", \"organization\"],\n      \"description\": \"Security type for the flow webhook endpoint\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of steps in the flow\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n      \
  \    },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"action\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"component\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"key\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"key\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flow was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the flow was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/flow.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Flow
---
