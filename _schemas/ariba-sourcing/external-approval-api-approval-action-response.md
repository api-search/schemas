---
description: Response from submitting an approval action.
layout: schema
name: ApprovalActionResponse
properties_list:
- description: Task identifier.
  name: taskId
  type: string
- description: Action submitted.
  name: action
  type: string
- description: Result status.
  name: status
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-action-response-schema.json
slug: external-approval-api-approval-action-response
source_filename: external-approval-api-approval-action-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-action-response-schema.json\",\n  \"title\": \"ApprovalActionResponse\",\n  \"description\": \"Response from submitting an approval action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\",\n      \"example\": \"TASK-500123\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action submitted.\",\n      \"example\": \"approve\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Result status.\",\n      \"example\": \"submitted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-action-response-schema.json
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
title: ApprovalActionResponse
---
