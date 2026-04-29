---
description: Details about an external approval task.
layout: schema
name: ApprovalTask
properties_list:
- description: Task identifier.
  name: taskId
  type: string
- description: Type of document being approved.
  name: documentType
  type: string
- description: Document identifier.
  name: documentId
  type: string
- description: Task status.
  name: status
  type: string
- description: Approval request entries with approver details.
  name: approvalRequests
  type: array
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-task-schema.json
slug: external-approval-api-approval-task
source_filename: external-approval-api-approval-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-task-schema.json\",\n  \"title\": \"ApprovalTask\",\n  \"description\": \"Details about an external approval task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\",\n      \"example\": \"TASK-500123\"\n    },\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of document being approved.\",\n      \"example\": \"RFXDocument\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Document identifier.\",\n      \"example\": \"DOC-001234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Task status.\",\n      \"example\": \"pending\"\n    },\n    \"approvalRequests\": {\n      \"type\":\
  \ \"array\",\n      \"description\": \"Approval request entries with approver details.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApprovalRequest\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-task-schema.json
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
title: ApprovalTask
---
