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
