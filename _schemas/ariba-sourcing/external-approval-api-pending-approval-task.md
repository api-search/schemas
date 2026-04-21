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
