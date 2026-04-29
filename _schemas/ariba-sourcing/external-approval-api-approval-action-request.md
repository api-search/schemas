---
description: Request body for submitting an approval action.
layout: schema
name: ApprovalActionRequest
properties_list:
- description: Task identifier.
  name: taskId
  type: string
- description: Action to take.
  name: action
  type: string
- description: User ID submitting the action.
  name: userId
  type: string
- description: Optional comment for the action.
  name: comment
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-action-request-schema.json
slug: external-approval-api-approval-action-request
source_filename: external-approval-api-approval-action-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-action-request-schema.json\",\n  \"title\": \"ApprovalActionRequest\",\n  \"description\": \"Request body for submitting an approval action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\",\n      \"example\": \"TASK-500123\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action to take.\",\n      \"enum\": [\n        \"approve\",\n        \"deny\"\n      ],\n      \"example\": \"approve\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User ID submitting the action.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment for\
  \ the action.\",\n      \"example\": \"Approved per procurement policy.\"\n    }\n  },\n  \"required\": [\n    \"taskId\",\n    \"action\",\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-action-request-schema.json
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
title: ApprovalActionRequest
---
