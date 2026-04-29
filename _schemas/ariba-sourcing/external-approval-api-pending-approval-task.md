---
description: A pending external approval task.
layout: schema
name: PendingApprovalTask
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
- description: User assigned to this task.
  name: assignedTo
  type: string
- description: Task status.
  name: status
  type: string
- description: Full URL to view the approvable in the SAP Ariba UI.
  name: fullURL
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-pending-approval-task-schema.json
slug: external-approval-api-pending-approval-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-pending-approval-task-schema.json\",\n  \"title\": \"PendingApprovalTask\",\n  \"description\": \"A pending external approval task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\",\n      \"example\": \"TASK-500123\"\n    },\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of document being approved.\",\n      \"example\": \"RFXDocument\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Document identifier.\",\n      \"example\": \"DOC-001234\"\n    },\n    \"assignedTo\": {\n      \"type\": \"string\",\n      \"description\": \"User assigned to this task.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"\
  status\": {\n      \"type\": \"string\",\n      \"description\": \"Task status.\",\n      \"example\": \"pending\"\n    },\n    \"fullURL\": {\n      \"type\": \"string\",\n      \"description\": \"Full URL to view the approvable in the SAP Ariba UI.\",\n      \"example\": \"https://mycompany-T.sourcing.ariba.com/Sourcing/main/ad/taskWorkspace\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-pending-approval-task-schema.json
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
title: PendingApprovalTask
---
