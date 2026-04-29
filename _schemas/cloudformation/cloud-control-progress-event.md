---
description: Represents the current status of a resource operation request.
layout: schema
name: ProgressEvent
properties_list:
- description: The resource type name.
  name: TypeName
  type: string
- description: The primary identifier for the resource.
  name: Identifier
  type: string
- description: The unique token representing this resource operation request. Use this token with GetResourceRequestStatus to check operation progress.
  name: RequestToken
  type: string
- description: The unique token for hooks processing.
  name: HooksRequestToken
  type: string
- description: The resource operation type.
  name: Operation
  type: string
- description: The current status of the resource operation request.
  name: OperationStatus
  type: string
- description: When the resource operation request was initiated (Unix timestamp).
  name: EventTime
  type: number
- description: A JSON string representing the resource model.
  name: ResourceModel
  type: string
- description: A message explaining the current status.
  name: StatusMessage
  type: string
- description: The error code if the operation failed.
  name: ErrorCode
  type: string
- description: When to retry the operation (Unix timestamp).
  name: RetryAfter
  type: number
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloud-control-progress-event-schema.json
slug: cloud-control-progress-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProgressEvent\",\n  \"type\": \"object\",\n  \"description\": \"Represents the current status of a resource operation request.\",\n  \"properties\": {\n    \"TypeName\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type name.\"\n    },\n    \"Identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The primary identifier for the resource.\"\n    },\n    \"RequestToken\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token representing this resource operation request. Use this token with GetResourceRequestStatus to check operation progress.\"\n    },\n    \"HooksRequestToken\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token for hooks processing.\"\n    },\n    \"Operation\": {\n      \"type\": \"string\",\n      \"description\": \"The resource operation type.\"\n    },\n    \"OperationStatus\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The current status of the resource operation request.\"\n    },\n    \"EventTime\": {\n      \"type\": \"number\",\n      \"description\": \"When the resource operation request was initiated (Unix timestamp).\"\n    },\n    \"ResourceModel\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON string representing the resource model.\"\n    },\n    \"StatusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A message explaining the current status.\"\n    },\n    \"ErrorCode\": {\n      \"type\": \"string\",\n      \"description\": \"The error code if the operation failed.\"\n    },\n    \"RetryAfter\": {\n      \"type\": \"number\",\n      \"description\": \"When to retry the operation (Unix timestamp).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloud-control-progress-event-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: ProgressEvent
---
