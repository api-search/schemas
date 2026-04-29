---
description: Represents the progress of a hook invocation.
layout: schema
name: HookProgressEvent
properties_list:
- description: The type name of the hook.
  name: HookTypeName
  type: string
- description: The version of the hook type.
  name: HookTypeVersionId
  type: string
- description: The ARN of the hook type.
  name: HookTypeArn
  type: string
- description: The point in the provisioning workflow where the hook runs.
  name: InvocationPoint
  type: string
- description: The status of the hook invocation.
  name: HookStatus
  type: string
- description: The time the hook event occurred.
  name: HookEventTime
  type: number
- description: A message about the hook status.
  name: HookStatusMessage
  type: string
- description: How the hook failure should affect the overall operation.
  name: FailureMode
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloud-control-hook-progress-event-schema.json
slug: cloud-control-hook-progress-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HookProgressEvent\",\n  \"type\": \"object\",\n  \"description\": \"Represents the progress of a hook invocation.\",\n  \"properties\": {\n    \"HookTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"The type name of the hook.\"\n    },\n    \"HookTypeVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the hook type.\"\n    },\n    \"HookTypeArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the hook type.\"\n    },\n    \"InvocationPoint\": {\n      \"type\": \"string\",\n      \"description\": \"The point in the provisioning workflow where the hook runs.\"\n    },\n    \"HookStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the hook invocation.\"\n    },\n    \"HookEventTime\": {\n      \"type\": \"number\",\n      \"description\": \"The time the hook event occurred.\"\n    },\n    \"\
  HookStatusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A message about the hook status.\"\n    },\n    \"FailureMode\": {\n      \"type\": \"string\",\n      \"description\": \"How the hook failure should affect the overall operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloud-control-hook-progress-event-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: HookProgressEvent
---
